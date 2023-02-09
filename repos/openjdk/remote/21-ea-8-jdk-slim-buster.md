## `openjdk:21-ea-8-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:9c91b925be2992ac55432aa39fe734b4d58c760e86a8e4931c1f95def4657d53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-8-jdk-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:5f4a7b1f51779525d5f4e03487eb1bf0e9f663f05d48ae5373776207acc3caa1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230039564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5536f6ae3e4ef3ad25d04ba60680d8acafbd08d5071e4a7f584a5b97a5bc589f`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:48:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:48:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Thu, 09 Feb 2023 10:48:19 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:48:19 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:48:19 GMT
ENV JAVA_VERSION=21-ea+8
# Thu, 09 Feb 2023 10:48:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='ce77e229b2dc811e1231ab1197f851d3234e56cb9e9a26e9f1d7c0294eb09af8'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='c52c76023ce2b7202744161d92772f5bc21c6ada643b926c92d5a56b0d1c4664'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 09 Feb 2023 10:48:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2663dab68577a1981f0b3fc37a5c844efdc4fe97f8c1484772876d35aa3400c`  
		Last Modified: Thu, 09 Feb 2023 10:55:23 GMT  
		Size: 3.3 MB (3275972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d014e52b99082be828b5100dad602b6d0305686c80dadc8738a74998223c6629`  
		Last Modified: Thu, 09 Feb 2023 10:55:37 GMT  
		Size: 199.6 MB (199623061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-8-jdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:1935dfd5c1d74e28305ca0081697536f842e8db9f6b73017210f1acbff698ff9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227139666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c834a1ca0b0c72577209876cf32c8d131ba13e7929af314887cf2a1dda695fe`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:38 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Thu, 09 Feb 2023 10:08:38 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:08:38 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:08:38 GMT
ENV JAVA_VERSION=21-ea+8
# Thu, 09 Feb 2023 10:08:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='ce77e229b2dc811e1231ab1197f851d3234e56cb9e9a26e9f1d7c0294eb09af8'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='c52c76023ce2b7202744161d92772f5bc21c6ada643b926c92d5a56b0d1c4664'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 09 Feb 2023 10:08:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54e96f1e900b2dc0ee4c2a8e339dafaed86e5cd62d38154ed7c3cd08c3c69a6`  
		Last Modified: Thu, 09 Feb 2023 10:15:55 GMT  
		Size: 3.1 MB (3129383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498c319100b0d1a7c28225a5cd1f2164448d37088a5a6e462b98bf1482c98c50`  
		Last Modified: Thu, 09 Feb 2023 10:16:07 GMT  
		Size: 198.1 MB (198087458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
