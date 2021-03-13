## `clojure:openjdk-16-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:6a9bfe50ea5928d5db55a71b92b2c41f4a6e245784b70b803b1c92cfafaea746
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:20ef1b0278252fecdf6f4217337d1b6fc80628715c2e36254781da76d8313fa3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.6 MB (274617008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d3bd722ef8ea4fb17f4df9017601bdd5c4dfa8f524e8f1c95e8fba37c8a757`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Mar 2021 20:57:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 20:59:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 09 Mar 2021 20:59:55 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:59:55 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 20:59:56 GMT
ENV JAVA_VERSION=16
# Tue, 09 Mar 2021 21:00:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='e952958f16797ad7dc7cd8b724edd69ec7e0e0434537d80d6b5165193e33b931'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='273d3ae0ff14af801c5ffa71fd081f1cc505354f308ce11c77af55302c83d2bf'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 21:00:09 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:51:12 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 09 Mar 2021 21:51:13 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:51:13 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:51:18 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 09 Mar 2021 21:51:18 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 09 Mar 2021 21:51:18 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 09 Mar 2021 21:51:39 GMT
RUN boot
# Tue, 09 Mar 2021 21:51:39 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f1fbf102b7eaa0998133d35bbcc37641d4d23626a4a2673cb9a2393cb7c34c`  
		Last Modified: Tue, 09 Mar 2021 21:10:48 GMT  
		Size: 3.3 MB (3268548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ccab748b0184655ff89a7b21f0844c8635ebb7eaa0ac2c0d5e2fe441fc8c52`  
		Last Modified: Tue, 09 Mar 2021 21:14:52 GMT  
		Size: 185.2 MB (185153170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6133d77e102145c919ba3f25e4ebd5dac96f0fadff5b184398211d7958ffdd50`  
		Last Modified: Tue, 09 Mar 2021 22:07:12 GMT  
		Size: 279.7 KB (279663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5271064c7b0215787db266ef44b696475521694c0a37cca9f607b0d20df1d2`  
		Last Modified: Tue, 09 Mar 2021 22:07:16 GMT  
		Size: 58.8 MB (58820485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-boot-2.8.3-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9dcce9654a86f1a4857f6ce1967f4e693a56357a29de1e76391dbacec5692c47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.6 MB (267604756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50093bca7a18fab16b91ff2d68cbcec759a02af961b9f8bf93dd0fb065e26f65`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:37:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Fri, 12 Mar 2021 06:37:06 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:37:07 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 06:37:07 GMT
ENV JAVA_VERSION=16
# Fri, 12 Mar 2021 06:37:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='e952958f16797ad7dc7cd8b724edd69ec7e0e0434537d80d6b5165193e33b931'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='273d3ae0ff14af801c5ffa71fd081f1cc505354f308ce11c77af55302c83d2bf'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 06:37:31 GMT
CMD ["jshell"]
# Sat, 13 Mar 2021 01:05:18 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 13 Mar 2021 01:05:19 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 13 Mar 2021 01:05:20 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 01:05:32 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 13 Mar 2021 01:05:33 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 13 Mar 2021 01:05:34 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 13 Mar 2021 01:06:00 GMT
RUN boot
# Sat, 13 Mar 2021 01:06:02 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303a8d33f3a602102b6a15a1f7974fc79449cdcff2c2fa6709b56cd1ac792384`  
		Last Modified: Fri, 12 Mar 2021 06:45:08 GMT  
		Size: 3.1 MB (3118728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814158e9e12f222a40698e829a10f013b36cb5516d9873c5c28425841d14cd98`  
		Last Modified: Fri, 12 Mar 2021 06:47:01 GMT  
		Size: 179.5 MB (179529577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0394627491bcdce9f6a6c8090102ac7ee6894b46777a6a51235371bd8b83982`  
		Last Modified: Sat, 13 Mar 2021 01:19:23 GMT  
		Size: 279.6 KB (279644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ff62926b35d15b5d940785a6f6c80efc6650a0e6bee02b38ec6a1e690bc7f5`  
		Last Modified: Sat, 13 Mar 2021 01:19:28 GMT  
		Size: 58.8 MB (58820295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
