## `clojure:openjdk-18-boot-bullseye`

```console
$ docker pull clojure@sha256:3f433fb70fa2afb38a6928e3b33282e1ef156337727a6810f4b9d0d73b43ba17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:b171005d5193d250f12ff14fe8fede1a9a9b6331235d6635ea719807577f3609
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.2 MB (387163953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0359975f7a0219850e7e84d5b56291b6f77c859c7ea2198645e40787ad44de72`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:07 GMT
ADD file:e777355768c63f735e5458c7e0ada7f556f27d0493b3af35dc7c34f9c4294ea9 in / 
# Thu, 02 Dec 2021 02:48:08 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:39:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:40:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:28:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:28:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:28:56 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:28:56 GMT
ENV LANG=C.UTF-8
# Sat, 18 Dec 2021 04:10:48 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 04:11:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 18 Dec 2021 04:11:06 GMT
CMD ["jshell"]
# Sat, 18 Dec 2021 06:54:25 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 18 Dec 2021 06:54:25 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 18 Dec 2021 06:54:25 GMT
WORKDIR /tmp
# Sat, 18 Dec 2021 06:54:26 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sat, 18 Dec 2021 06:54:26 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 18 Dec 2021 06:54:26 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 18 Dec 2021 06:54:50 GMT
RUN boot
# Sat, 18 Dec 2021 06:54:50 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 18 Dec 2021 06:54:50 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 18 Dec 2021 06:54:50 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:5e0b432e8ba9d9029a000e627840b98ffc1ed0c5172075b7d3e869be0df0fe9b`  
		Last Modified: Thu, 02 Dec 2021 02:53:18 GMT  
		Size: 54.9 MB (54932878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84cfd68b5cea612a8343c346bfa5bd6c486769010d12f7ec86b23c74887feb2`  
		Last Modified: Thu, 02 Dec 2021 03:49:22 GMT  
		Size: 5.2 MB (5153424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b8f2315954535f1e27cd13d777e73da4a787b0aebf4241d225beff3c91cbb1`  
		Last Modified: Thu, 02 Dec 2021 03:49:23 GMT  
		Size: 10.9 MB (10871995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fa43a7e793a76c198e8d45d8810394e1cfc943b2673d7fcf5a6fdc4f45b3`  
		Last Modified: Thu, 02 Dec 2021 03:49:46 GMT  
		Size: 54.6 MB (54567844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718dc22cae0d908da735cfc9f467980c8c89a8029b7fe88b1f442d6df8c8a305`  
		Last Modified: Thu, 02 Dec 2021 11:46:40 GMT  
		Size: 14.1 MB (14071762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cbbffaef4da332948b187b6b2a27f0cc1b1d60340e8c16c89c6fa454528bc2`  
		Last Modified: Sat, 18 Dec 2021 04:23:43 GMT  
		Size: 188.7 MB (188738231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821e79867ca06476c613be158985d5e49b008f64665aab1ef2a6211f8e2c19f7`  
		Last Modified: Sat, 18 Dec 2021 07:01:26 GMT  
		Size: 6.9 KB (6897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec952b6c5d30ff6e98eff0842b34b64332ea562367832712a81c35d0afc36b4`  
		Last Modified: Sat, 18 Dec 2021 07:01:30 GMT  
		Size: 58.8 MB (58820516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd560ca2b5bd619189219d1dd93e188bd6ac126c081fc015268863ac95bcfd35`  
		Last Modified: Sat, 18 Dec 2021 07:01:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5640f920d8b076ced975df68b3c01d06a664fc12e16653acdc447aaf79875a41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385908967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438a58f8bebc81673cb12e1bbf454ba3196a589d0d80935bd94a919be20b3005`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 02 Dec 2021 08:07:54 GMT
ADD file:998dc1c35eeeed1ddf46156aeb337fb9b8cbb4855caf994201167a1061f4ecbf in / 
# Thu, 02 Dec 2021 08:07:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:53:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 09:53:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:01:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:01:46 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:01:47 GMT
ENV LANG=C.UTF-8
# Fri, 17 Dec 2021 23:44:01 GMT
ENV JAVA_VERSION=18-ea+28
# Fri, 17 Dec 2021 23:44:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 17 Dec 2021 23:44:13 GMT
CMD ["jshell"]
# Sat, 18 Dec 2021 00:35:41 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 18 Dec 2021 00:35:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 18 Dec 2021 00:35:42 GMT
WORKDIR /tmp
# Sat, 18 Dec 2021 00:35:44 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sat, 18 Dec 2021 00:35:45 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 18 Dec 2021 00:35:45 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 18 Dec 2021 00:36:00 GMT
RUN boot
# Sat, 18 Dec 2021 00:36:01 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 18 Dec 2021 00:36:01 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 18 Dec 2021 00:36:02 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6476cb406b24c94f24348db05d154b814b14ee38860dea1625080e7e08295a80`  
		Last Modified: Thu, 02 Dec 2021 08:40:14 GMT  
		Size: 53.6 MB (53619027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96565d527970b1cc982493f96d6b317b1fbfdd7bf0ea6fd58d44942bb4f597c5`  
		Last Modified: Thu, 02 Dec 2021 10:02:24 GMT  
		Size: 4.9 MB (4937631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c15f93136056df893ba8088992a38e90dc37210fd6ebb712413fd045c58de`  
		Last Modified: Thu, 02 Dec 2021 10:02:25 GMT  
		Size: 10.7 MB (10655914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee42e24e52cb2f9b50ab14328865298f5ae6ac159219db890afc6366ec641a46`  
		Last Modified: Thu, 02 Dec 2021 10:02:46 GMT  
		Size: 54.7 MB (54669690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009bf5207e45bc64cf6af7e65c157106b890f904af8e570d361dfa9675e87778`  
		Last Modified: Thu, 02 Dec 2021 11:22:35 GMT  
		Size: 15.5 MB (15524985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77b2a926c3efa79ae0bf6c66e5867e24f41ed71e6c80e6dc7fe8c0e43646f54`  
		Last Modified: Sat, 18 Dec 2021 00:02:45 GMT  
		Size: 187.7 MB (187678712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69a02fddeae4b01fedb756cab3242f0abcd156ced9fcf0cee0880a92173f27a`  
		Last Modified: Sat, 18 Dec 2021 00:45:47 GMT  
		Size: 6.9 KB (6873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b68e79f8bb2e40c7a167693c5393d9ebbb62f543da5532705e5bb3753d66d37`  
		Last Modified: Sat, 18 Dec 2021 00:45:52 GMT  
		Size: 58.8 MB (58815729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4397ae50a51b05c8a4eeee6813c57ff0f44ce874037086066f94dddccd446e3`  
		Last Modified: Sat, 18 Dec 2021 00:45:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
