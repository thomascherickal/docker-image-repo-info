## `clojure:openjdk-19-boot`

```console
$ docker pull clojure@sha256:ec1b5ee329780859b687f52f7bc68ed2492e76f42ff97f0612adafd8b6874927
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-19-boot` - linux; amd64

```console
$ docker pull clojure@sha256:1b9202c6fc8fbf561ebad0ae33ce34a226faeb8fd2658711875ecc8deea50515
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.5 MB (285485567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b6a9421787204cdc579137bd1994b505b6500579eb767409e591156a125944`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:21:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:21:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 01 Mar 2022 14:21:07 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 14:21:07 GMT
ENV LANG=C.UTF-8
# Sat, 05 Mar 2022 02:04:43 GMT
ENV JAVA_VERSION=19-ea+12
# Sat, 05 Mar 2022 02:04:57 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/12/GPL/openjdk-19-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='5bb24f4e4ddcb4a2a81f9a32174afccc0a94f0ba3fbd7b8e48212fc6091199ef'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/12/GPL/openjdk-19-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='f1b776f48f8612b3a60854a24d329a174266c2db4a9552a078652a6c495f4775'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Mar 2022 02:04:57 GMT
CMD ["jshell"]
# Sat, 05 Mar 2022 02:35:36 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 05 Mar 2022 02:35:36 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 05 Mar 2022 02:35:36 GMT
WORKDIR /tmp
# Sat, 05 Mar 2022 02:35:41 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 05 Mar 2022 02:35:41 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 05 Mar 2022 02:35:41 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 05 Mar 2022 02:36:17 GMT
RUN boot
# Sat, 05 Mar 2022 02:36:18 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 05 Mar 2022 02:36:18 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 05 Mar 2022 02:36:18 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8366d5a4a5f71bf009ed651eb5566bf81bcd61ddaa4a2541fc65505bb076ca`  
		Last Modified: Tue, 01 Mar 2022 14:40:45 GMT  
		Size: 1.6 MB (1582090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e455babf6ed5f6b3acc998ce5a2bc3c021779936059636acc115643d44a5a8`  
		Last Modified: Sat, 05 Mar 2022 02:13:32 GMT  
		Size: 193.4 MB (193432868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc8cc7e4138eb01b8994d6b1f2218c2adb77f4e37fb2bfc8ac9f36cdbe66d2b`  
		Last Modified: Sat, 05 Mar 2022 02:41:59 GMT  
		Size: 283.1 KB (283074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74ee553ca32739bb27204a59ce42d062373c9598894fdf6186fb7d17776515a`  
		Last Modified: Sat, 05 Mar 2022 02:42:03 GMT  
		Size: 58.8 MB (58820733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd8dce25fea09b9f8a15caec280e2ccfc500f1a3d26a8ea81fa68b641081aec`  
		Last Modified: Sat, 05 Mar 2022 02:41:59 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-19-boot` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:de03cacf13e225f8605df9fdd98d236d90ba4d48b1d7a44967c20a4344a7205a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282752871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e08ff0eda5fd9d59a76bb1de36dc86d5872a8d643c43302a606fc739abde8e14`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:48:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:48:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 01 Mar 2022 13:48:14 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 13:48:15 GMT
ENV LANG=C.UTF-8
# Sat, 05 Mar 2022 02:56:22 GMT
ENV JAVA_VERSION=19-ea+12
# Sat, 05 Mar 2022 02:56:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/12/GPL/openjdk-19-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='5bb24f4e4ddcb4a2a81f9a32174afccc0a94f0ba3fbd7b8e48212fc6091199ef'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/12/GPL/openjdk-19-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='f1b776f48f8612b3a60854a24d329a174266c2db4a9552a078652a6c495f4775'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Mar 2022 02:56:37 GMT
CMD ["jshell"]
# Sat, 05 Mar 2022 03:47:40 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 05 Mar 2022 03:47:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 05 Mar 2022 03:47:42 GMT
WORKDIR /tmp
# Sat, 05 Mar 2022 03:47:47 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 05 Mar 2022 03:47:48 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 05 Mar 2022 03:47:49 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 05 Mar 2022 03:48:26 GMT
RUN boot
# Sat, 05 Mar 2022 03:48:27 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 05 Mar 2022 03:48:27 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 05 Mar 2022 03:48:28 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eee4a8201309b4b9bb0e0e0efc8d45265ae39d932512f5edb149b65eaf107d9`  
		Last Modified: Tue, 01 Mar 2022 14:12:59 GMT  
		Size: 1.6 MB (1565936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf4e6b628187d07f73ef4822f44699d7a4bea814a07f209a52b02dc780f4d22`  
		Last Modified: Sat, 05 Mar 2022 03:11:10 GMT  
		Size: 192.2 MB (192245697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164ee269787acb8049364e7a4aff48752615b02b8c46527f6fd466b448cc45f8`  
		Last Modified: Sat, 05 Mar 2022 03:57:43 GMT  
		Size: 67.2 KB (67231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fb35a7701438a4c228375e112dae15ab4e402440ae46d2a1b1b44cdc1fec5d`  
		Last Modified: Sat, 05 Mar 2022 03:57:47 GMT  
		Size: 58.8 MB (58816593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ee3bdd60a859fcda457755a46a427dd0796f6e9058bbb87e8f0a6a70b3f78d`  
		Last Modified: Sat, 05 Mar 2022 03:57:42 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
