## `clojure:openjdk-18-boot-2.8.3-buster`

```console
$ docker pull clojure@sha256:801c3318859eeeab219c1068d04fb81719a4a1933ee558b034386ec16e8178fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot-2.8.3-buster` - linux; amd64

```console
$ docker pull clojure@sha256:f9f869203e43c38ca7d8a7271c8f6cee1afae40e4ac2e2a2339faec3822bf11a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.4 MB (380415602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cf5d45440d2f5e67d7bbdfc0f0c0c7154309a6f84605550ce879f1b679b04d4`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:33:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:32:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:32:04 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:32:05 GMT
ENV LANG=C.UTF-8
# Tue, 14 Sep 2021 01:32:44 GMT
ENV JAVA_VERSION=18-ea+14
# Tue, 14 Sep 2021 01:32:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='6aee5779ac7488dbd6988658662ca683704ac98cee6b8dde8df3ddffac76142e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='88a106afe903b8f5d552ceae108294d8b36cbc0656a744f84525ccae542c5029'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Sep 2021 01:32:54 GMT
CMD ["jshell"]
# Tue, 14 Sep 2021 02:13:57 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 14 Sep 2021 02:13:57 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 14 Sep 2021 02:13:58 GMT
WORKDIR /tmp
# Tue, 14 Sep 2021 02:13:59 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Tue, 14 Sep 2021 02:13:59 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 14 Sep 2021 02:13:59 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 14 Sep 2021 02:14:49 GMT
RUN boot
# Tue, 14 Sep 2021 02:14:49 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e5f66f5d0e1c97622f33d44fb04efb42bd3562bdc3482537d121040c789f9a`  
		Last Modified: Fri, 03 Sep 2021 06:40:37 GMT  
		Size: 7.8 MB (7833606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c8f1c77d6674046d7deb41be1ca07f25cb43fd67f87e879ee79cc6586087f0`  
		Last Modified: Fri, 03 Sep 2021 06:40:37 GMT  
		Size: 10.0 MB (9997249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5095cab277710f0c2883844158323ad986c763ffc37353ddff874dd85585d9b6`  
		Last Modified: Fri, 03 Sep 2021 06:40:55 GMT  
		Size: 51.8 MB (51840968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee27e112836c56c7a7f0e8a1986512005c433ddddbe7aaff39133b826a04844`  
		Last Modified: Fri, 03 Sep 2021 08:50:02 GMT  
		Size: 13.9 MB (13921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89857ce3f39017cfcae77a5aa5ef0065be326d5b27d066c4140b4c775eca4aea`  
		Last Modified: Tue, 14 Sep 2021 01:41:47 GMT  
		Size: 187.6 MB (187558832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1c862d5499ffd2202f8f5d5f907654a9d207aac53d5ab97e66427c9ce02e41`  
		Last Modified: Tue, 14 Sep 2021 02:24:06 GMT  
		Size: 6.9 KB (6918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e0fa630b27c0e79518d338eec17246f7f4ea916bd1b8dbc89c9da0921a6aac`  
		Last Modified: Tue, 14 Sep 2021 02:24:15 GMT  
		Size: 58.8 MB (58820876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot-2.8.3-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:dcccad84b14e0e8da69e68f759fbce81a0a14fb14738871e2248e35c26e4d768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.9 MB (378868503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4f552eaf278220331870005888a5f0f2a0727f9ac2a2054c828272d2099360`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:44 GMT
ADD file:1d6e5f5349752ab5c5888d38637821d2943472188c06bd14ea2bdf7a676ea19b in / 
# Fri, 03 Sep 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:33:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 04:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:45:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:45:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 10:45:01 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 10:45:01 GMT
ENV LANG=C.UTF-8
# Tue, 14 Sep 2021 01:59:04 GMT
ENV JAVA_VERSION=18-ea+14
# Tue, 14 Sep 2021 01:59:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='6aee5779ac7488dbd6988658662ca683704ac98cee6b8dde8df3ddffac76142e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='88a106afe903b8f5d552ceae108294d8b36cbc0656a744f84525ccae542c5029'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Sep 2021 01:59:13 GMT
CMD ["jshell"]
# Tue, 14 Sep 2021 02:38:50 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 14 Sep 2021 02:38:51 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 14 Sep 2021 02:38:51 GMT
WORKDIR /tmp
# Tue, 14 Sep 2021 02:38:57 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Tue, 14 Sep 2021 02:38:57 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 14 Sep 2021 02:38:57 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 14 Sep 2021 02:39:27 GMT
RUN boot
# Tue, 14 Sep 2021 02:39:28 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e3c1991bf0816d8624d8191a43732b869478319ed39c5f218e5878ed1ee05d58`  
		Last Modified: Fri, 03 Sep 2021 00:49:16 GMT  
		Size: 49.2 MB (49222144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529bf6c2a9fdb0edf93a87f6fbc959069a0068fe2ed046af546fca48e8ed6ffe`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 7.7 MB (7695770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9703bfb802a7157134df39897b2625906f8057c03e52daa3e8298ca41dfd7b`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 10.0 MB (9984267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a64745ecb3a1d83570e6c503995c0eb3f97176e23bd91210bf235e5646a4e96`  
		Last Modified: Fri, 03 Sep 2021 04:42:38 GMT  
		Size: 52.2 MB (52167858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a619afbd5fbf8751bdfe501f2c76be064cd35c66bc77c681698f60417a131a`  
		Last Modified: Fri, 03 Sep 2021 11:05:51 GMT  
		Size: 14.7 MB (14673457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e8c1323638d2f6705a6849427671a35427d900a540166991096421996a880f`  
		Last Modified: Tue, 14 Sep 2021 02:15:11 GMT  
		Size: 186.3 MB (186297602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeedd5f892f299255ee1acf6633377613e9bf731b4c5e62fc6bd2ede7b8effdf`  
		Last Modified: Tue, 14 Sep 2021 02:51:43 GMT  
		Size: 6.9 KB (6917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1bf136995091764f1a68e626dde31c5d842c1d137d4239a13ee176a4350848`  
		Last Modified: Tue, 14 Sep 2021 02:51:48 GMT  
		Size: 58.8 MB (58820488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
