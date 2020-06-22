## `openjdk:16-ea-slim-buster`

```console
$ docker pull openjdk@sha256:436f15b688ac2ea7a5d0bd056096d8c876c505e219e3b6af5e13800f4395739d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-ea-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:1056b11375dc5e427daab2dda86485c1473b98aad21a7a6b6c1ec92369c5b30f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226484684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aaa52d3fcb9bf984148df3fbae8986ad3f5c7fc355ff34fe70c1189b9d54005`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 16:34:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:34:37 GMT
ENV LANG=C.UTF-8
# Thu, 18 Jun 2020 20:38:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 18 Jun 2020 20:38:48 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Jun 2020 20:38:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 22 Jun 2020 19:31:55 GMT
ENV JAVA_VERSION=16-ea+2
# Mon, 22 Jun 2020 19:32:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_linux-aarch64_bin.tar.gz; 			downloadSha256=c166b3aeb4901a4b082b99e73234b4a7603ae123505a20aca7d7ab907a25903d; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_linux-x64_bin.tar.gz; 			downloadSha256=5a29aad9b578aaa3427522f4e777e273b3c92f8b7befa8e5c8819741e168ec1c; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Mon, 22 Jun 2020 19:32:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65306eca6b8ea03d29cd8d10a31e9d7a6a1cf8766fe4ca3913e75e00fc47be79`  
		Last Modified: Tue, 09 Jun 2020 16:41:33 GMT  
		Size: 3.2 MB (3248452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f76d4aac25607b3b14d08740c1c6d3f6d8b7439aa088c24728f1638d686267`  
		Last Modified: Thu, 18 Jun 2020 20:42:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f01d0c754cbfbdb726a2a35a8c15c9107c8b2fa3a1a96901c18ffbefdc3d37`  
		Last Modified: Mon, 22 Jun 2020 19:37:21 GMT  
		Size: 196.1 MB (196137756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2ba2e979c5257c570a55e734d37eff35c7c2d446c701b9e99da3438d088c80c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204192368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fad10995abaaf8fa01199545d1f00f2138c7190aa4ffed75d1c58a39636d6fc`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 13:43:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 13:43:09 GMT
ENV LANG=C.UTF-8
# Thu, 18 Jun 2020 23:57:00 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 18 Jun 2020 23:57:00 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Jun 2020 23:57:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 22 Jun 2020 20:04:26 GMT
ENV JAVA_VERSION=16-ea+2
# Mon, 22 Jun 2020 20:04:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_linux-aarch64_bin.tar.gz; 			downloadSha256=c166b3aeb4901a4b082b99e73234b4a7603ae123505a20aca7d7ab907a25903d; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_linux-x64_bin.tar.gz; 			downloadSha256=5a29aad9b578aaa3427522f4e777e273b3c92f8b7befa8e5c8819741e168ec1c; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Mon, 22 Jun 2020 20:04:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e741745c97e3614499fd6b9013ef0b77c85309673e303a5c5bfa4a09bd38c41a`  
		Last Modified: Tue, 09 Jun 2020 13:48:30 GMT  
		Size: 3.1 MB (3101468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba1239ad73ea22f721a3cf41797404827d972a8c4e148ac1e765a7ae652ac64`  
		Last Modified: Fri, 19 Jun 2020 00:00:47 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd0b6eb4e2873c515f8ff16b16ca3efadbefbbfcee7074809fbff570c9f9cf1`  
		Last Modified: Mon, 22 Jun 2020 20:10:17 GMT  
		Size: 175.2 MB (175232985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
