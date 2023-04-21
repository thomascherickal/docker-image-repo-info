## `openjdk:21-ea-bullseye`

```console
$ docker pull openjdk@sha256:c0cb5d3c90bc886ff5725604b5beecbb1f27814147fbae91edd4c929090f02ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:4e9a5644bd24e5ac2d03c83d16d4fdd4261021b3838e0703d591799a105d40fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.4 MB (341434815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c12acf0f44208243810eeb4cca48ccb9bda96bb6d956c7b8754674c83fec835`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:37:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 12 Apr 2023 09:37:56 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 09:37:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Apr 2023 20:07:33 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 20:07:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5af95497753fbc33981f5ab1267fbd3be57e4095ceca9806490a25b56f819007'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='d08fe17feea7fa18c4e9ee9918496974d0194d1fac9a485d47cc2d30601c3682'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Apr 2023 20:07:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b89f3c7f7da8adf032a33a75d1b659cee33179ecb88ea0ba75e4fc58ebe63a6`  
		Last Modified: Wed, 12 Apr 2023 07:57:46 GMT  
		Size: 54.6 MB (54584801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8e057755186cfddd700ee42c11d1751039420315372369491644d2f5bfda04`  
		Last Modified: Wed, 12 Apr 2023 09:39:55 GMT  
		Size: 14.1 MB (14072018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68462a89c7b5a6885891c5d72140c542d5b0c8d9a5964a2eed49c7ced4951037`  
		Last Modified: Fri, 21 Apr 2023 20:10:32 GMT  
		Size: 201.7 MB (201681815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:cf2827ff042bbb407bc7508692cdf038aef7bf8295443c83e156c6872c0d1b2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.0 MB (339984746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6531c5b674e133be23e161366463858ef9f6be47c48b3a5f3fd519ea1de0ea2a`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:10:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:10:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 12 Apr 2023 05:10:41 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 05:10:41 GMT
ENV LANG=C.UTF-8
# Fri, 21 Apr 2023 20:22:54 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 20:23:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5af95497753fbc33981f5ab1267fbd3be57e4095ceca9806490a25b56f819007'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='d08fe17feea7fa18c4e9ee9918496974d0194d1fac9a485d47cc2d30601c3682'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Apr 2023 20:23:06 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f993d5b17f32f4b8a535c25e182e5d8412625beee450e513ca57036e8fdd6dc`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 54.7 MB (54676038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09cb5578d3115a65cc6337102cf310454aa8eef83438795a15e17d95122657d`  
		Last Modified: Wed, 12 Apr 2023 05:12:33 GMT  
		Size: 15.5 MB (15529043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3474d60dccbe99faf471cadf206ef248747650694c7a0550b2cd4114aaa0b7`  
		Last Modified: Fri, 21 Apr 2023 20:25:37 GMT  
		Size: 200.0 MB (200047729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
