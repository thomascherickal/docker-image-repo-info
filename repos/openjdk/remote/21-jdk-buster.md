## `openjdk:21-jdk-buster`

```console
$ docker pull openjdk@sha256:a5b151c575ca00701d83f6142a4643015daab19e86e1ed9a5b96f0dc15d801d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-jdk-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:eb588fcb09b600238efd2d5dd94d2ad324b19cc3b7d1e3b5abf1b408535e7783
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.2 MB (333171267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f9b01dff55e9cd97e1be879d6269f4ebe59456603f9f337b85a50a372fb52b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 05:06:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Dec 2022 00:34:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 14 Dec 2022 00:34:02 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:34:02 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 23:30:51 GMT
ENV JAVA_VERSION=21-ea+2
# Fri, 16 Dec 2022 23:31:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='8070902e5bfbb71a4e7c723bb0439faeb9f3127e1fb048f7ed4e6a5abc5a3505'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='011358a514a8d4030c36bbd5b7d7fb5c404f326498f4c832ee5f890fff8709db'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Dec 2022 23:31:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5db87f5b42af9f258f14f367616814cb9b518ea0141f46bdd2706bb256d408`  
		Last Modified: Tue, 06 Dec 2022 02:23:06 GMT  
		Size: 51.8 MB (51844146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38c5a27848987ad9841d24cd247491c27004097057dd37f061d2a5613506fc0`  
		Last Modified: Tue, 06 Dec 2022 05:11:58 GMT  
		Size: 13.9 MB (13927569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e12be3c7b4f3d26475e38b3929aabf5aacf61513dc0dd3514887b670da5fc1e`  
		Last Modified: Fri, 16 Dec 2022 23:39:08 GMT  
		Size: 199.1 MB (199089900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e28deb77cb8a5ad35390471bd2e6f8fa89ac8816f2da4fee7fc36c1ff484c094
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.4 MB (331403138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20bde59b92a4a28794c1d312e3ded63ed547db4488373b09c53d5c5239350d2`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:24 GMT
ADD file:2deba7c04e28d01997b865f366cdc8d38a80aa39720c4e4d1fc581ac17e8ce4a in / 
# Tue, 06 Dec 2022 01:40:25 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:06:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:06:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:27:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Dec 2022 00:54:34 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 14 Dec 2022 00:54:34 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:54:34 GMT
ENV LANG=C.UTF-8
# Sat, 17 Dec 2022 00:26:40 GMT
ENV JAVA_VERSION=21-ea+2
# Sat, 17 Dec 2022 00:26:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='8070902e5bfbb71a4e7c723bb0439faeb9f3127e1fb048f7ed4e6a5abc5a3505'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='011358a514a8d4030c36bbd5b7d7fb5c404f326498f4c832ee5f890fff8709db'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 17 Dec 2022 00:26:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:47d0ec2abdb05569eada58143acd16d47ee4b07a33535544cf5bf267bde20cc3`  
		Last Modified: Tue, 06 Dec 2022 01:44:13 GMT  
		Size: 49.2 MB (49233737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626af93612b745b80b7a70ce5fb9fc87baa4761919cb1bef555440f52c2942dd`  
		Last Modified: Tue, 06 Dec 2022 02:12:50 GMT  
		Size: 7.7 MB (7727211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823037cfb749c6f284b1368decc632435d3a62f1190e4657fb94151c7c4473a1`  
		Last Modified: Tue, 06 Dec 2022 02:12:50 GMT  
		Size: 10.0 MB (10003593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dda455e0271e29e2bce16f33d91b99bedfe8975de9c6d245b2e196257212a8`  
		Last Modified: Tue, 06 Dec 2022 02:13:04 GMT  
		Size: 52.2 MB (52172425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea555784730da4cd1d5f477240291ddde4e8949a7708d22f4177478fc03388c5`  
		Last Modified: Tue, 06 Dec 2022 04:32:57 GMT  
		Size: 14.7 MB (14673004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cad52b21bb6eaa8cfafb47b38d9f228dbf7062139fdb4d07fc38b24d3c2bf36`  
		Last Modified: Sat, 17 Dec 2022 00:34:52 GMT  
		Size: 197.6 MB (197593168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
