## `clojure:openjdk-18-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:bc2d99ea1992c9bd7d79265b1bc72f25314b9c41fbfee2e9a067fc2837d61d07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:f91ec4e7fa0e31b30df708058fe98fa45f6044bdc3cb2ee2d4608d2d97563325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278539443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9609b973a39eb922c4baa8f77da92fe891452b68c7c12eb8090b65e270bcc6`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 22:58:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 22:59:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 21 Dec 2021 22:59:58 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 22:59:59 GMT
ENV LANG=C.UTF-8
# Sat, 08 Jan 2022 00:33:25 GMT
ENV JAVA_VERSION=18-ea+30
# Sat, 08 Jan 2022 00:33:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='4e34f307a3d9b1c020a864e863a0f47c701036592d634da55c6e548d101526ed'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='10fd6ab1369a4cd536570c4cccfd2aead86bfd733fd7171de74e0b979c04b96e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 08 Jan 2022 00:33:44 GMT
CMD ["jshell"]
# Sat, 08 Jan 2022 01:13:56 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 08 Jan 2022 01:13:56 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 08 Jan 2022 01:13:56 GMT
WORKDIR /tmp
# Sat, 08 Jan 2022 01:14:02 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 08 Jan 2022 01:14:02 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 08 Jan 2022 01:14:02 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 08 Jan 2022 01:14:32 GMT
RUN boot
# Sat, 08 Jan 2022 01:14:33 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 08 Jan 2022 01:14:33 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 08 Jan 2022 01:14:33 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c983bcc370920d99695dc288c345343be841987206e4ce762a4e7599f28c96`  
		Last Modified: Tue, 21 Dec 2021 23:16:09 GMT  
		Size: 3.3 MB (3269567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bcba58e36d795fdad1beb5d8f665d39284c505d6a4228c0f4a681a710f17b5`  
		Last Modified: Sat, 08 Jan 2022 00:53:54 GMT  
		Size: 189.0 MB (189015344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9dfc5326392bce31d3400057fbb2a7bff00d3fc12248b31c0d9d964d96b8a0`  
		Last Modified: Sat, 08 Jan 2022 01:23:40 GMT  
		Size: 279.8 KB (279842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58622931c6f9c59bc525338a9e8afb64d6a733122771d2bd408482acc0012ed6`  
		Last Modified: Sat, 08 Jan 2022 01:23:44 GMT  
		Size: 58.8 MB (58820562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e76d5a92a0a91f2ac11152a0e05610ea0c8260f4585496ee25807ae6e6c4277`  
		Last Modified: Sat, 08 Jan 2022 01:23:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot-2.8.3-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ee2236aaf32d85c268a368378f23d2b20d2939881112cc539bebb432824c0f99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.7 MB (275668066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:672a5e607b395f15738616326ff4926e83e980d828f8e084e69b6f34302f4b04`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:54:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:56:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 21 Dec 2021 02:56:42 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:56:43 GMT
ENV LANG=C.UTF-8
# Sat, 08 Jan 2022 00:54:43 GMT
ENV JAVA_VERSION=18-ea+30
# Sat, 08 Jan 2022 00:54:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='4e34f307a3d9b1c020a864e863a0f47c701036592d634da55c6e548d101526ed'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='10fd6ab1369a4cd536570c4cccfd2aead86bfd733fd7171de74e0b979c04b96e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 08 Jan 2022 00:54:58 GMT
CMD ["jshell"]
# Sat, 08 Jan 2022 01:40:51 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 08 Jan 2022 01:40:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 08 Jan 2022 01:40:53 GMT
WORKDIR /tmp
# Sat, 08 Jan 2022 01:40:58 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 08 Jan 2022 01:40:59 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 08 Jan 2022 01:41:00 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 08 Jan 2022 01:41:42 GMT
RUN boot
# Sat, 08 Jan 2022 01:41:44 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 08 Jan 2022 01:41:44 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 08 Jan 2022 01:41:45 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c74145b5f237a66007b7c0d55f2ffe3d54c07bf5e09c19bebd4ec94b00005e`  
		Last Modified: Tue, 21 Dec 2021 03:17:41 GMT  
		Size: 3.1 MB (3118854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecb573e5dc4ca1638b5f266680463985b997bae2d3a292d76021b950826f831`  
		Last Modified: Sat, 08 Jan 2022 01:14:47 GMT  
		Size: 187.7 MB (187741332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5936b47d7fee38478fa6c34dcb50a69b5dcf11fed6c4fc5d7677a3b2812f29e`  
		Last Modified: Sat, 08 Jan 2022 01:53:20 GMT  
		Size: 67.5 KB (67504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cfcebb138aff9cbfed86d98364eb25c85d098a19edd2881ef76343679e30ff`  
		Last Modified: Sat, 08 Jan 2022 01:53:26 GMT  
		Size: 58.8 MB (58816821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962209018fca14226c64b928558dd2d5b471ee656a4c76996c313c5cf715cfad`  
		Last Modified: Sat, 08 Jan 2022 01:53:20 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
