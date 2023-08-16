## `openjdk:21-rc-bookworm`

```console
$ docker pull openjdk@sha256:26a919d2d8ec0003e11b231b88064e286583f25354be22f53681ab06b62be8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-rc-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:0ef76cbc98a868216586b1c8a0cc6195fad6648054f831b4a785f93b41048599
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.7 MB (358698638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01da9e6a6f16cdc1c68d47fbd46bb644ebbd1026b9a74a689265fb12d6253232`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:30 GMT
ADD file:3a6d159d80cb8abfacda5873c243a6ae635ff603708febc4df51f8eec26d3de7 in / 
# Wed, 16 Aug 2023 00:59:31 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 06:58:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:17:36 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 16 Aug 2023 15:17:36 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 15:17:36 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:17:36 GMT
ENV JAVA_VERSION=21
# Wed, 16 Aug 2023 15:17:47 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 16 Aug 2023 15:17:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:de4cac68b6165c40cf6f8b30417948c31be03a968e233e55ee40221553a5e570`  
		Last Modified: Wed, 16 Aug 2023 01:04:06 GMT  
		Size: 49.6 MB (49557399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31b0195ec5f04dfc78eca9d73b5d223fc36a29f54ee888bc4e0615b5839e692`  
		Last Modified: Wed, 16 Aug 2023 07:12:39 GMT  
		Size: 24.0 MB (24030511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1fd34c30b75e7edb20c2fd09a9862697f302ef9ae357e521ef3c84d5534e3f`  
		Last Modified: Wed, 16 Aug 2023 07:12:59 GMT  
		Size: 64.1 MB (64112171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97d4e9887f878c0c4f34c6d9782b3a13202d338b31c939c9f823e0c29022247`  
		Last Modified: Wed, 16 Aug 2023 15:19:32 GMT  
		Size: 16.9 MB (16947339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a558feb6e61db8a560ee385415789df99fd1260df2d51f1f3d73e9635b6b790`  
		Last Modified: Wed, 16 Aug 2023 15:22:17 GMT  
		Size: 204.1 MB (204051218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-rc-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c22d407596c77a9a44dc05939ebce580657c8d1d23a527b3e8393b32a8647de7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.3 MB (357270259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1404902a8253af23caf808e61a0c31b852574dfd1ad3a1218c75796719959841`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:21:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:11:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:13:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 16 Aug 2023 04:13:46 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 04:13:46 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 04:13:46 GMT
ENV JAVA_VERSION=21
# Wed, 16 Aug 2023 04:14:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 16 Aug 2023 04:14:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1109a21287fa17dc866e87e8c6685113960cbb0379fee8f42b83de63c647`  
		Last Modified: Wed, 16 Aug 2023 01:38:47 GMT  
		Size: 64.0 MB (63988473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e1d2ce07002848455170902f2b6ea91a492e5b318bc6ae2fb7691c51b7e9ed`  
		Last Modified: Wed, 16 Aug 2023 04:16:10 GMT  
		Size: 17.7 MB (17729096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb42a933ddf4c1a9519184d898763be448e711ab1354e3c20d448aff1a1afa`  
		Last Modified: Wed, 16 Aug 2023 04:18:27 GMT  
		Size: 202.4 MB (202391334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
