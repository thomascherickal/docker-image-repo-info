## `openjdk:20-ea-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:c9977f112eb6de32191fe7ea3f7654a4cbf8ebeeac03b171468c8527e9006849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:d59ad618029bfe06965e50eff6df28f4ced4ed2f44ba1514adc75e9676967503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228930636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f5bfeb279c2f039267f4058eeb70f845aafb8372ad9a5a1b58132fa7b85bce`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:48:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:49:32 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Thu, 09 Feb 2023 10:49:32 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:49:33 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:49:33 GMT
ENV JAVA_VERSION=20-ea+34
# Thu, 09 Feb 2023 10:49:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='1c8e4809d7444903dfde02ef45821c1206a5d98c241c04280434ef9b5aca15ad'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e43b2f39d2b6359755a6cd26c01057b1b6d53c84d944fc3396500b2f21a15be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 09 Feb 2023 10:49:47 GMT
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
	-	`sha256:8f13aad3d6e580febe68527ebfb3dbfb6528b82bc6b5967e7cf253f2d4737877`  
		Last Modified: Thu, 09 Feb 2023 10:58:02 GMT  
		Size: 198.5 MB (198514133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:5f2adf9257142aa211cfd979992e8df4af8f35dae1c443afa574a1f85a218c88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226065841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb2d8df5037a1952bb744793cbe34aebd3eeb588847042f1d3f34c892b5eb3e`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:09:54 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Thu, 09 Feb 2023 10:09:54 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:09:54 GMT
ENV LANG=C.UTF-8
# Fri, 10 Feb 2023 01:59:27 GMT
ENV JAVA_VERSION=20-ea+35
# Fri, 10 Feb 2023 01:59:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/35/GPL/openjdk-20-ea+35_linux-x64_bin.tar.gz'; 			downloadSha256='2062453caf72cff8ad296b84d90108f2eb057d7415a5c7d109672fd6b613ef1f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/35/GPL/openjdk-20-ea+35_linux-aarch64_bin.tar.gz'; 			downloadSha256='65541ed26e56fe91b7d3ba703bde269e5568313e3e7168d2476455f03f460eda'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Feb 2023 01:59:41 GMT
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
	-	`sha256:a8240ce6cd708c524ec8313516a762ac98dbc0894463ec27112cd7dad82af441`  
		Last Modified: Fri, 10 Feb 2023 02:09:28 GMT  
		Size: 197.0 MB (197013633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
