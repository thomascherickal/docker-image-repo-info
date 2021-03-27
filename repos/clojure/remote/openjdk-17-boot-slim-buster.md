## `clojure:openjdk-17-boot-slim-buster`

```console
$ docker pull clojure@sha256:71a6ea1300ecd4e9f68aed23fd7afb79d922b3484400b9b066d5018f689845f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:c2a84704eb56a21492a5dfd5fcaf963566d2fea9329da199ff0b9b762b4a8480
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275415428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b3cb4cb6098661aa7bf058c82f1c3ae90eb81f8ffdd6857010d78827fe779e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 19:24:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 19:24:33 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 26 Mar 2021 19:24:33 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 19:24:33 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 19:24:33 GMT
ENV JAVA_VERSION=17-ea+15
# Fri, 26 Mar 2021 19:24:48 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='da690c53a8d23b278b4878acf414b0d95ca40dd1533d08ce313589cf1df1c9c3'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93178b313750b38e1bbc811b989dcee27d988cb223b30ba829122ecdbd08f403'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 19:24:49 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:11:44 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 26 Mar 2021 20:11:44 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 26 Mar 2021 20:11:44 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:11:50 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 26 Mar 2021 20:11:50 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 26 Mar 2021 20:11:50 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 26 Mar 2021 20:12:11 GMT
RUN boot
# Fri, 26 Mar 2021 20:12:11 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f37f3c8df9c4599e86451848bc7d181558d9106306657ffef1e8a59f44b7f7`  
		Last Modified: Fri, 26 Mar 2021 19:32:50 GMT  
		Size: 3.3 MB (3268744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d64f535a678982062036b0be2acf726821ecb53a9dfe2f57600648194e31c`  
		Last Modified: Fri, 26 Mar 2021 19:33:06 GMT  
		Size: 185.9 MB (185945734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54854e645b11546c7bd2f832f4a178906d727c2b307b6e62144edfc18b4c7a07`  
		Last Modified: Fri, 26 Mar 2021 20:22:48 GMT  
		Size: 279.6 KB (279643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac7875c0b2d2c91e558f7ef2fa0328e56860089164fdd50b591f8140cea089`  
		Last Modified: Fri, 26 Mar 2021 20:22:52 GMT  
		Size: 58.8 MB (58820311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:afd9ab7c081f9dc36546a0c39d6d841bcb48b5524da467713923ccc278c34fd6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.1 MB (270096199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a2621f2f89e6a874e75206acb5fd60f8bbdfe294337892f0784f37a85dfd064`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 19:43:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 19:43:15 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 26 Mar 2021 19:43:15 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 19:43:16 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 19:43:17 GMT
ENV JAVA_VERSION=17-ea+15
# Fri, 26 Mar 2021 19:43:57 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='da690c53a8d23b278b4878acf414b0d95ca40dd1533d08ce313589cf1df1c9c3'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93178b313750b38e1bbc811b989dcee27d988cb223b30ba829122ecdbd08f403'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 19:43:59 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:20:52 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 26 Mar 2021 20:20:53 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 26 Mar 2021 20:20:53 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:21:03 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 26 Mar 2021 20:21:04 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 26 Mar 2021 20:21:05 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 26 Mar 2021 20:21:27 GMT
RUN boot
# Fri, 26 Mar 2021 20:21:28 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d8de9377aa4bd4c66d812b6226ebe8ebcb1dbbbdf3be6e3e9d0ea7363e0d3`  
		Last Modified: Fri, 26 Mar 2021 19:50:29 GMT  
		Size: 3.1 MB (3118857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8a684536826257d175f2a7600e0046e7e7d2c61220d1c7441161448cd4f4a5`  
		Last Modified: Fri, 26 Mar 2021 19:50:54 GMT  
		Size: 182.0 MB (182021333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e4193ca4124e1436976a4df7b0e6ad48c7607fbe43ec2c010e5dc8ddb8c801`  
		Last Modified: Fri, 26 Mar 2021 20:28:44 GMT  
		Size: 279.5 KB (279513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab118b847f34e9ceaa77b90fa1037bfbb95a8f9b07ac997e33f563f6361b42ae`  
		Last Modified: Fri, 26 Mar 2021 20:28:51 GMT  
		Size: 58.8 MB (58820112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
