## `openjdk:19-ea-slim-buster`

```console
$ docker pull openjdk@sha256:8fe029bd8756656aa2cab17d33e6002a1dcda614a12cef2d33309265959ceb03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:3f16bcc1816f00a2f8e3a73ed3a3d115f865ee3454272362651c0f9c0e59a73e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226968980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e55b4f1746a311fdfc1d4a51419d35a76456b1ba821dc47b6038b89df92e230b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:24 GMT
ADD file:81dbfe4f9df4d280f7580380c0c5c93ba71fedba17b3072d2b7b4bce127f88a9 in / 
# Tue, 02 Aug 2022 01:20:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:48:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:50:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 02 Aug 2022 05:50:04 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 05:50:04 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 22:54:25 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:54:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 22:54:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:751ef25978b2971e15496369695ba51ed5b1b9aaca7e37b18a173d754d1ca820`  
		Last Modified: Tue, 02 Aug 2022 01:25:00 GMT  
		Size: 27.1 MB (27140083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140e22108c7d39a72fc1f5f3ba4ffdd55836614e9c53175f5d43ada8b6bbaacc`  
		Last Modified: Tue, 02 Aug 2022 06:02:41 GMT  
		Size: 3.3 MB (3273367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a93da09195aa356765d0af647573f3e5dd9898b3c35902ca082762c9fb6e1`  
		Last Modified: Mon, 08 Aug 2022 23:07:27 GMT  
		Size: 196.6 MB (196555530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f0573e27dc8af24133687783c1d1bbd01d78c181c806f3831c76d9da85afcec7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224236000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7648ffa841c010b923a39d8d08f9bae37e0766a5c9a788f37c0f79dea8ab048a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:44:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 02 Aug 2022 04:44:54 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 04:44:55 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 23:34:28 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 23:34:42 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 23:34:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c6f3c25c4deaf78673b1fd4ca615f7a3d33a177d1d101f83a1700e34bc27f1`  
		Last Modified: Tue, 02 Aug 2022 05:05:08 GMT  
		Size: 3.1 MB (3126019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6013b3059bfa383eafc3392836db1f5fff7b95c342323320eb073208a7e11c09`  
		Last Modified: Mon, 08 Aug 2022 23:54:22 GMT  
		Size: 195.2 MB (195195618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
