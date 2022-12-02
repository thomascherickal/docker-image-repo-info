## `openjdk:20-slim-bullseye`

```console
$ docker pull openjdk@sha256:5c26f21a52c54156aa6e8d8aae5f5ac88349ff8490a6f0dd939a8c5caf18a3a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:64966724c2a9ccd37b9f1e0839f1e0d0a24758f5e624c6c62a0c1b3060571703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231323086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b0c9210f3709d663b17a1ab07c4bdce323d673f3c6767b2dd833abee8d9288`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:37:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:37:09 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 15 Nov 2022 13:37:09 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 13:37:09 GMT
ENV LANG=C.UTF-8
# Fri, 02 Dec 2022 00:22:05 GMT
ENV JAVA_VERSION=20-ea+26
# Fri, 02 Dec 2022 00:22:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Dec 2022 00:22:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54e66bc569588bf6945416d9455248d373e1db9ffe9428a75b3963b798662d6`  
		Last Modified: Tue, 15 Nov 2022 13:42:10 GMT  
		Size: 1.6 MB (1583981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d465869bc41d66cdc0feecaa2b1da97dbf2cc87a890b7679ae9bede6d4e`  
		Last Modified: Fri, 02 Dec 2022 00:27:18 GMT  
		Size: 198.3 MB (198326475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:6a3d8d10b11449ff20622d0fe41f1b4fb09d01a71d84cbef941b523c9812efca
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.5 MB (228503543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e73968cae1f3841d0a43722f8e5cf9ae9048b48ea939e9ab505e703528074f6f`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:59:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:59:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 15 Nov 2022 06:59:21 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 06:59:21 GMT
ENV LANG=C.UTF-8
# Thu, 01 Dec 2022 23:44:04 GMT
ENV JAVA_VERSION=20-ea+26
# Thu, 01 Dec 2022 23:44:16 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Dec 2022 23:44:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb8ead4542ac0732ce51843584ff03141aa14c30f7161cc4856f3caa5d7a95`  
		Last Modified: Tue, 15 Nov 2022 07:04:17 GMT  
		Size: 1.6 MB (1567467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3d61973ac6c97c3a4b7d6f02552e4620c7954c252b01f2977b86471b3d7319`  
		Last Modified: Thu, 01 Dec 2022 23:49:16 GMT  
		Size: 196.9 MB (196875471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
