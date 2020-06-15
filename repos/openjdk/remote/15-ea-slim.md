## `openjdk:15-ea-slim`

```console
$ docker pull openjdk@sha256:2a44693cae6ca2251db029967f2765eccfe4013e7357202328608713b3fcbdef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:15-ea-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:10368bbbc25cb56ed29013eba1bc20f5a7f5c065fb664ad356302f96099b50e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226052281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6338a0e60269038e5ed85dec41ba3f934e570f0f03be7beccfa1741382f05ee7`
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
# Tue, 09 Jun 2020 16:34:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Tue, 09 Jun 2020 16:34:37 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:34:38 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 10 Jun 2020 06:10:37 GMT
ENV JAVA_VERSION=15-ea+26
# Wed, 10 Jun 2020 06:10:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/26/GPL/openjdk-15-ea+26_linux-aarch64_bin.tar.gz; 			downloadSha256=3167b538bffc43925847159facbf5b880321065db6e55e5d5baeaeff9dca4c2d; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/26/GPL/openjdk-15-ea+26_linux-x64_bin.tar.gz; 			downloadSha256=62fa98366f85cf37cba4758dfd6b683b397d60af3a130943de54dcddd3a4b1d8; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Wed, 10 Jun 2020 06:10:55 GMT
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
	-	`sha256:483b95dcfbd46dbdc1240666a5cb96e2881dbdecfff2f75f23bd5932127de1bd`  
		Last Modified: Tue, 09 Jun 2020 16:41:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2246db1bb9c4342afc4d5ac0fea9fdc9c0afb8edd0080a99cd0135ae92dd70`  
		Last Modified: Wed, 10 Jun 2020 06:13:55 GMT  
		Size: 195.7 MB (195705354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-ea-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:54672c350207d61244c07d00503b0509ac35ec7cb20c9355b0bbf7729d3353b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.1 MB (204110523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1722e1be54033547121636b9afa4eae88ccdca9630bc5a3cdbe1c246c32fef`
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
# Tue, 09 Jun 2020 13:43:10 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Tue, 09 Jun 2020 13:43:11 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 13:43:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 15 Jun 2020 20:47:08 GMT
ENV JAVA_VERSION=15-ea+27
# Mon, 15 Jun 2020 20:47:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/27/GPL/openjdk-15-ea+27_linux-aarch64_bin.tar.gz; 			downloadSha256=9195473bcb8e4ceaf0113cdb7b3dad468f3c045ebb9c0ce326bf01818c089269; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/27/GPL/openjdk-15-ea+27_linux-x64_bin.tar.gz; 			downloadSha256=db20094a26993699a0c6beb10dc5d07d9e708ab1fc0bfb7aff637944c3319374; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Mon, 15 Jun 2020 20:47:30 GMT
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
	-	`sha256:38432c521f52b4151d59e0725fe9c21d40cfb8e92964962e6dbe2a957f515e95`  
		Last Modified: Tue, 09 Jun 2020 13:48:29 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672454d667e3df51b6e4a72585931fddefab9e5cb19745596aecd18e3a1cc8a9`  
		Last Modified: Mon, 15 Jun 2020 20:50:25 GMT  
		Size: 175.2 MB (175151141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
