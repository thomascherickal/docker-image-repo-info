## `clojure:openjdk-16-boot-buster`

```console
$ docker pull clojure@sha256:fdfd5a14985523e422ec4b6657e4a8516ef776904fb932ef69030a1c6d59256d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-boot-buster` - linux; amd64

```console
$ docker pull clojure@sha256:bd934cda2ed1d946af21b31cb4e1217963155d3e4c6700f75a5df643ba63ee37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.7 MB (377663884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76497dc5cb3438c4fa0811a545c022d1a9007c8dd884bcf5aadb6ed94f957bc4`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:57:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:51:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 10:53:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 12 Jan 2021 10:53:59 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 10:54:01 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 23 Jan 2021 01:24:26 GMT
ENV JAVA_VERSION=16-ea+33
# Sat, 23 Jan 2021 01:24:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/33/GPL/openjdk-16-ea+33_linux-aarch64_bin.tar.gz; 			downloadSha256=1da1b96306a0ede9e1c7b4284772b5de3c9f8f08f895e082f561f5f3c86ea3be; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/33/GPL/openjdk-16-ea+33_linux-x64_bin.tar.gz; 			downloadSha256=ba2ac6ccca898cd63090d768b89a95fba76b6303a55c41e851d75dd0c5afcee8; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 23 Jan 2021 01:24:40 GMT
CMD ["jshell"]
# Sat, 23 Jan 2021 01:52:50 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 23 Jan 2021 01:52:50 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 23 Jan 2021 01:52:50 GMT
WORKDIR /tmp
# Sat, 23 Jan 2021 01:52:51 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sat, 23 Jan 2021 01:52:51 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 23 Jan 2021 01:52:52 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 23 Jan 2021 01:53:11 GMT
RUN boot
# Sat, 23 Jan 2021 01:53:11 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fd949ed9338da3c1e09f9b75408c214368c637c448e0fd839467f6f7717b5`  
		Last Modified: Tue, 12 Jan 2021 04:06:20 GMT  
		Size: 51.8 MB (51830144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb84f8603a0e9c23b65bd7aa67bbb9d1388f3a82a3522afa5e7862966510804`  
		Last Modified: Tue, 12 Jan 2021 11:06:40 GMT  
		Size: 13.9 MB (13920374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042d0ad48d9ed73ecbeefdb5fa16ef77cc979a0163a79248a3f8ab560621917f`  
		Last Modified: Tue, 12 Jan 2021 11:08:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a4df19a62c127d8db76188a4b0cafbf784827106e7f153892062205df8ad3a`  
		Last Modified: Sat, 23 Jan 2021 01:32:53 GMT  
		Size: 184.9 MB (184878411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23c7403298d9b4aff057aa5bfad0fc09363966febc7d750c030a64085be395e`  
		Last Modified: Sat, 23 Jan 2021 01:56:25 GMT  
		Size: 6.9 KB (6901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b648ff81a48f7071d9fb38d372c830f44a979da5915d84b1d4f3172892bc90`  
		Last Modified: Sat, 23 Jan 2021 01:56:29 GMT  
		Size: 58.8 MB (58820280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-boot-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5be76023bdf34f70c8cef0c4e553ef4a7b1b47e57000570b061e12da64089df3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.8 MB (371765308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a39f886d563b96280d59a5eb38390653f1d07e962ebb61f15be623b3f55d8b9f`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:24:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:20:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:20:04 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 18:21:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 12 Jan 2021 18:21:42 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 18:21:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 23 Jan 2021 01:47:03 GMT
ENV JAVA_VERSION=16-ea+33
# Sat, 23 Jan 2021 01:47:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/33/GPL/openjdk-16-ea+33_linux-aarch64_bin.tar.gz; 			downloadSha256=1da1b96306a0ede9e1c7b4284772b5de3c9f8f08f895e082f561f5f3c86ea3be; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/33/GPL/openjdk-16-ea+33_linux-x64_bin.tar.gz; 			downloadSha256=ba2ac6ccca898cd63090d768b89a95fba76b6303a55c41e851d75dd0c5afcee8; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 23 Jan 2021 01:47:48 GMT
CMD ["jshell"]
# Sat, 23 Jan 2021 02:20:09 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 23 Jan 2021 02:20:10 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 23 Jan 2021 02:20:11 GMT
WORKDIR /tmp
# Sat, 23 Jan 2021 02:20:13 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sat, 23 Jan 2021 02:20:13 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 23 Jan 2021 02:20:14 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 23 Jan 2021 02:20:38 GMT
RUN boot
# Sat, 23 Jan 2021 02:20:39 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53f70a43c3c83782c39cad75aa09ccddb893b3fd54762416fca4d48a3b44b5`  
		Last Modified: Tue, 12 Jan 2021 01:38:54 GMT  
		Size: 52.2 MB (52163502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe81219355ad3760f5108d0ebcf47afc7df2d4d28b077d0dcddb6046c2fba47`  
		Last Modified: Tue, 12 Jan 2021 18:31:19 GMT  
		Size: 14.7 MB (14673793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4b07e9dbcd72d92c589e809e3f5e12b6db5915d9b56520c874a33cb3582b9a`  
		Last Modified: Tue, 12 Jan 2021 18:32:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b30a11277107cce3db42503ec7dfaf30ee1b549dd3eead3357b5bc77249946`  
		Last Modified: Sat, 23 Jan 2021 01:56:23 GMT  
		Size: 179.3 MB (179250249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc55b6d3a47b302aa886c83be5b5e68929555a8f54b2d4e30366744a098a30f5`  
		Last Modified: Sat, 23 Jan 2021 02:24:31 GMT  
		Size: 6.9 KB (6901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb5d0b894d05e25d4c09d38273ca9258d6ab21a95f32afd77656c6a2ca4c29`  
		Last Modified: Sat, 23 Jan 2021 02:24:38 GMT  
		Size: 58.8 MB (58820264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
