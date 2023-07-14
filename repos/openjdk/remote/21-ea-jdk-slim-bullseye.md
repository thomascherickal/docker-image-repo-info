## `openjdk:21-ea-jdk-slim-bullseye`

```console
$ docker pull openjdk@sha256:927f7f6fa48c6a48507c6f9ccb8b089153792294ada7c992db8544074cfd1d7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-jdk-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:8e2205013399d1867dab6509e51ff3b20c068f8dccaf565043621bc079cc7b66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237237837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25d3ca2bc017c64be8bf770ec5eeb00e5a3745a9c8d27bbe5700940d9cedbd9`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:53:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:54:54 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 04 Jul 2023 01:54:54 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 01:54:54 GMT
ENV LANG=C.UTF-8
# Fri, 14 Jul 2023 00:35:59 GMT
ENV JAVA_VERSION=21-ea+31
# Fri, 14 Jul 2023 00:36:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/31/GPL/openjdk-21-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='e2f42a80cedd4a2e59f7bd479fd308aa71a53b785012b79efa570bfc7ec21a12'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/31/GPL/openjdk-21-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='4ea543bd3c33a75f02b74f6a838e577c43e8e150cac353e22c70898b3ba119c8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 Jul 2023 00:36:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae78b1797b5f8b06d429ce740e570a94adf8b155152e2e3faa83a259c83894cc`  
		Last Modified: Tue, 04 Jul 2023 01:59:02 GMT  
		Size: 1.6 MB (1582468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e553634a6d261253643706246a36add3a04aed9e03d744fced16277bde2a0b00`  
		Last Modified: Fri, 14 Jul 2023 00:43:56 GMT  
		Size: 204.2 MB (204237981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:51397c3348f1764b06a8959d8b598e62db2ad0592d5b77cc46cdc78405200e41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234216150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd5a428da72356df6722a31381dad84df2e064338d5f8e4d5b80a96f0a87ab5`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 13:27:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:29:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 04 Jul 2023 13:29:13 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 13:29:13 GMT
ENV LANG=C.UTF-8
# Fri, 14 Jul 2023 00:47:27 GMT
ENV JAVA_VERSION=21-ea+31
# Fri, 14 Jul 2023 00:47:38 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/31/GPL/openjdk-21-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='e2f42a80cedd4a2e59f7bd479fd308aa71a53b785012b79efa570bfc7ec21a12'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/31/GPL/openjdk-21-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='4ea543bd3c33a75f02b74f6a838e577c43e8e150cac353e22c70898b3ba119c8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 Jul 2023 00:47:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb66ab3fe3ab74b42fe268bde056fcbee783ef1979718ffa94fa05e09805b822`  
		Last Modified: Tue, 04 Jul 2023 13:31:59 GMT  
		Size: 1.6 MB (1566385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f245fefde71052676c7752e339b04333778fde31ac7e74f144eb56d8e49421`  
		Last Modified: Fri, 14 Jul 2023 00:54:55 GMT  
		Size: 202.6 MB (202586808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
