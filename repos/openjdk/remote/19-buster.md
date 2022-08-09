## `openjdk:19-buster`

```console
$ docker pull openjdk@sha256:9e5fba59ef244747808fc7613e1c9ec7674171f3c2f65c9f8c5e80d5d387997c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:1d47c5971333e410f1cf18c2e5ecb7579508a06b3eb033661d13dc138159feaf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.4 MB (330353414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc07c8a3b6ed4147c68f65a2aa50905974d5338c93a362b129cab2cf24ab3105`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:14 GMT
ADD file:647206e0e9c1daa306e4ebbdc26c3ef1840dd316ba4ffea905d17b0858e58e34 in / 
# Tue, 02 Aug 2022 01:20:14 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:48:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:48:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:48:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:48:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:49:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 02 Aug 2022 05:49:50 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 05:49:50 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 22:54:11 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:54:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 22:54:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7e6a53d1988fa8e19db6bcfc96ee6783afb079c38dbe047528e691815d19a9fa`  
		Last Modified: Tue, 02 Aug 2022 01:24:34 GMT  
		Size: 50.4 MB (50440980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe4e1c58b4af82939a918665dd1e7b5b636dd73c710b4bccb530edbb15470d2`  
		Last Modified: Tue, 02 Aug 2022 02:19:38 GMT  
		Size: 7.9 MB (7856856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc915d298757b72963f0d061cc16ca4925e9f4481446b87a5297b4043ffc8033`  
		Last Modified: Tue, 02 Aug 2022 02:19:38 GMT  
		Size: 10.0 MB (9998020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08b88f29371de7c9ac165381b7426349760f6af3f205e8716426fafce4a1ff2`  
		Last Modified: Tue, 02 Aug 2022 02:19:56 GMT  
		Size: 51.8 MB (51843653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8030644bcacbb6a4560d02d857bcc61ce786528a842649f701e44543172852`  
		Last Modified: Tue, 02 Aug 2022 06:02:08 GMT  
		Size: 13.9 MB (13921448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1130d77507771d5b5e1ca00adc9834b729307b5b5a0ff325fe91235e46bf9bb9`  
		Last Modified: Mon, 08 Aug 2022 23:06:52 GMT  
		Size: 196.3 MB (196292457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:5adbbb493e48095ab87eb6ec2ead22b2e15997bcfed595c54329795c9f790f8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.7 MB (328699827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e95e88e9b3f48bc0c337d3b23d918bc2031890c10f9a3811ffc874598a2a1a6`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:49 GMT
ADD file:dfd7e3791fa0512f0f7c9cc8530233d6bc1b0a586a3656fd3950ea386754808a in / 
# Tue, 02 Aug 2022 00:40:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:25:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:25:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:26:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:42:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:44:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 02 Aug 2022 04:44:32 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 04:44:33 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 23:34:09 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 23:34:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 23:34:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:71209d5eb534b9e48223962276993c68559f68e230f73c8a0efc2a2998362bd9`  
		Last Modified: Tue, 02 Aug 2022 00:46:28 GMT  
		Size: 49.2 MB (49229053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31ca5ccee8fca6610f14b5ed35ac33bb5f545532b6583e1461037a083c3d87b`  
		Last Modified: Tue, 02 Aug 2022 01:45:50 GMT  
		Size: 7.7 MB (7719992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de8e1f96ccb825d3be85704be7218044a19ff05ea1eea0222e8c942fbf6f8f`  
		Last Modified: Tue, 02 Aug 2022 01:45:50 GMT  
		Size: 9.8 MB (9768645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965555a6fd3b7a1727fd927269ea37139a09652f2545ea1c825b36af887f2713`  
		Last Modified: Tue, 02 Aug 2022 01:46:10 GMT  
		Size: 52.2 MB (52175033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5412b4b2cbcf161ed600cfb50b7e757f4207cdcb027137699a952aa9d3a20fa3`  
		Last Modified: Tue, 02 Aug 2022 05:04:28 GMT  
		Size: 14.7 MB (14670842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd398647e85b07e58bf2b69c3004030a90fbdf91ce5295ce9765a4fc6f6bdd2`  
		Last Modified: Mon, 08 Aug 2022 23:53:39 GMT  
		Size: 195.1 MB (195136262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
