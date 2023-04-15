## `openjdk:21-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:aee3d9f29b7c7e63871880aa8767a6725df678506c57d6c82cb4efc95ea614c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-jdk-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:936e6308deae407f36dccd89999bf20f8b128364f9f3c978b19152a60762e457
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.2 MB (232217750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9763c918185b9fe28356e9999615e3bcb5c4aa16d90277756a54209a074f257`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:25 GMT
ADD file:e614539607055bdbde0cc1a94ef9783fe3627c8553ef1b21071ecb5c27ea27e4 in / 
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:39:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:39:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 12 Apr 2023 09:39:08 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 09:39:08 GMT
ENV LANG=C.UTF-8
# Sat, 15 Apr 2023 00:31:27 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:31:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1c6d7b740ced597243d8c05f823f81728a618c73ffa4cbe28a6d3e2eba02ce00'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='b0009295c1ef02c743fc272b654b11bd506714e8efedc881295a1de74e87d8a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 15 Apr 2023 00:31:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9fbefa3370776b7ec7633cf07efc14cc24e0c0cd53893ad0e7e3f44ffdc1bedb`  
		Last Modified: Wed, 12 Apr 2023 00:24:22 GMT  
		Size: 27.1 MB (27138920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e35bb669fa393f13e7b4c100af1023e9c2da16c731aff14e3fd9e83c7cfe2a8`  
		Last Modified: Wed, 12 Apr 2023 09:41:34 GMT  
		Size: 3.3 MB (3278764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e4197f0243545fee77338a59516177f6a88bf5ff41a769ee69f8213622cd1f`  
		Last Modified: Sat, 15 Apr 2023 00:35:14 GMT  
		Size: 201.8 MB (201800066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:34e7cefaeac7e1f741247f66d426f997e52f51c75b620741d6d9a962c0439fb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229207969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5ed71bf43e4703b85ffee33feb2a5aeb54b4077a684df65351157f11a9e1d7`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:02 GMT
ADD file:39d4ef5cc48487567b857a8527ab3c106b5099eafffbeaa8b70df450fb8409e3 in / 
# Wed, 12 Apr 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:11:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:11:47 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 12 Apr 2023 05:11:47 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 05:11:47 GMT
ENV LANG=C.UTF-8
# Sat, 15 Apr 2023 00:56:43 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:56:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1c6d7b740ced597243d8c05f823f81728a618c73ffa4cbe28a6d3e2eba02ce00'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='b0009295c1ef02c743fc272b654b11bd506714e8efedc881295a1de74e87d8a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 15 Apr 2023 00:56:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:27bec964ec41cf69bd5df2ffd45c27623ae4bb0eb6f9f366179f7ac9b47d9840`  
		Last Modified: Wed, 12 Apr 2023 00:43:11 GMT  
		Size: 25.9 MB (25922011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbe87b3c027f2b1952babc2b86de6d9f2011dfb0410c3f340d15409fba01477`  
		Last Modified: Wed, 12 Apr 2023 05:14:03 GMT  
		Size: 3.1 MB (3131734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fa17a1720d32e567fa7e6f83c071557bb2c8f31da9d030add03eb320eacf4c`  
		Last Modified: Sat, 15 Apr 2023 01:00:13 GMT  
		Size: 200.2 MB (200154224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
