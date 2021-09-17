## `openjdk:18-ea-bullseye`

```console
$ docker pull openjdk@sha256:7cb2268906aa6cd7d93c39d06d1e36ffae12d74731a1dd6c188ab675a89d8f3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:43bdc1e6cbc3bdaabb724594490b88dc42c53f35eab94cfbb69f5b8d4161a50e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.5 MB (327458297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff340c4572a680c277287e9544bb9fbbcf01f5d594c24fb9c5238df999d3a9e5`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:07 GMT
ADD file:1fedf68870782f1b44cd50691444aab4061cc0c70f24e5fabe9c562cc46eb9af in / 
# Fri, 03 Sep 2021 01:21:08 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:31:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:31:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:30:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:30:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:30:45 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 19:33:37 GMT
ENV JAVA_VERSION=18-ea+15
# Fri, 17 Sep 2021 19:33:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/15/GPL/openjdk-18-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='d04e7163eb9519d4c918acc60d1f92fd7b6ff28bb0a43d7019790590b120725c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/15/GPL/openjdk-18-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='7a154bf56a56e4c4a4cdc6b5542e916b81baca431de262fa1a07e07ca313bd5e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 17 Sep 2021 19:33:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:955615a668ce169f8a1443fc6b6e6215f43fe0babfb4790712a2d3171f34d366`  
		Last Modified: Fri, 03 Sep 2021 01:26:55 GMT  
		Size: 54.9 MB (54926871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2756ef5f69a5190f4308619e0f446d95f5515eef4a814dbad0bcebbbbc7b25a8`  
		Last Modified: Fri, 03 Sep 2021 06:39:22 GMT  
		Size: 5.2 MB (5153100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ea9f2bd51e53a455297e0631e18a72a86d7e2c8e1807176e80f991bde5d64`  
		Last Modified: Fri, 03 Sep 2021 06:39:23 GMT  
		Size: 10.9 MB (10871687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b0a22ee906271a6ce9ddd1754fdd7d3b59078e0b57b6cc054c7ed7ac301587`  
		Last Modified: Fri, 03 Sep 2021 06:39:45 GMT  
		Size: 54.6 MB (54566834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b79c82cab03ddf5fc88cf1ab0550217980b866ec12c52b0f16751bc45be87b6`  
		Last Modified: Fri, 03 Sep 2021 08:48:24 GMT  
		Size: 14.1 MB (14071678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5745aa9a7add397b1f7b194d7f8ffe29b53792e9834cc086453b7e72d21c56`  
		Last Modified: Fri, 17 Sep 2021 19:44:32 GMT  
		Size: 187.9 MB (187868127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:0384124de0768a997473ca5feecb105f4dd3add629d8fd32025680ef34e6ed9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.4 MB (326421548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ea86570755358cd1f01dd9484bd48cbcf195653622263ffa99219e2f072c9e2`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:18 GMT
ADD file:0b1ff9dcb90d6b787179d2e43ca534c39e0372227a3af198bab158a89fb2c966 in / 
# Fri, 03 Sep 2021 00:40:19 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:32:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 04:32:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:44:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:44:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 10:44:07 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 10:44:07 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 19:17:08 GMT
ENV JAVA_VERSION=18-ea+15
# Fri, 17 Sep 2021 19:17:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/15/GPL/openjdk-18-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='d04e7163eb9519d4c918acc60d1f92fd7b6ff28bb0a43d7019790590b120725c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/15/GPL/openjdk-18-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='7a154bf56a56e4c4a4cdc6b5542e916b81baca431de262fa1a07e07ca313bd5e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 17 Sep 2021 19:17:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ffacddc51d82196acb1d49f2e3c13601fc16c61c995a860b450d23b000353ca1`  
		Last Modified: Fri, 03 Sep 2021 00:48:17 GMT  
		Size: 53.6 MB (53613054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f80252dfabbfc5bdf4862b9fa8d2de7110ac4a6f08bf30e6f574f6243d0c93d`  
		Last Modified: Fri, 03 Sep 2021 04:40:56 GMT  
		Size: 5.1 MB (5142543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138e2c18ad04e197e8431cfc2923456979d5b0cfb9c6549a62bcd3732d77bd03`  
		Last Modified: Fri, 03 Sep 2021 04:40:56 GMT  
		Size: 10.9 MB (10872696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9597521670e83c9cc67fab06b99d41fef6d1d65c0515c50154a74e2e4f4c7fc5`  
		Last Modified: Fri, 03 Sep 2021 04:41:20 GMT  
		Size: 54.7 MB (54669941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b20165388200285f501d4e258530008a43aa4efc936f6775d1d396ca814e39b`  
		Last Modified: Fri, 03 Sep 2021 11:04:06 GMT  
		Size: 15.5 MB (15526421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d97bd6da1f1babb42ecdd0325673574170c3892ab2865769374871882e26e`  
		Last Modified: Fri, 17 Sep 2021 19:32:19 GMT  
		Size: 186.6 MB (186596893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
