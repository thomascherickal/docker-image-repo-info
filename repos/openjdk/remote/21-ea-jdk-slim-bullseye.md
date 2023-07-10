## `openjdk:21-ea-jdk-slim-bullseye`

```console
$ docker pull openjdk@sha256:e7c1705b8cd4a5572dd704dcee1ead9218726687528cc6a8924be032e81b9272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-jdk-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:bc01f07f7df30c8529782a2b95ebd87d64508481a99cce6c64c24e407e313b94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237242392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21d5c461aa74fb68b58a2ec90677a415177baab8c161fa39a1e4506475489aeb`
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
# Mon, 10 Jul 2023 20:49:31 GMT
ENV JAVA_VERSION=21-ea+30
# Mon, 10 Jul 2023 20:49:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='c35a1f2906d502e9f75a975165f4c86e29167ca8cc2d9d25b5351b46d90d4ab7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='ae690af5ffa639feba3bc04fc804480cdbc40b4099890c9d28dceac8f58f0426'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 10 Jul 2023 20:49:45 GMT
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
	-	`sha256:6c7413e1a1f5612148eb57e32c733c1e9f1b0072e59aa37e4fad4870dc6323a4`  
		Last Modified: Mon, 10 Jul 2023 20:57:36 GMT  
		Size: 204.2 MB (204242536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:58a0071323cff94b53745e9985fe47917cd73ed9bbc7e3925e9d0ec781aec5dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234220032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7629faf1cae6ae35d9d7b85a50386cd83290b854515a6aae46fb147a25ac3ab`
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
# Mon, 10 Jul 2023 21:35:55 GMT
ENV JAVA_VERSION=21-ea+30
# Mon, 10 Jul 2023 21:36:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='c35a1f2906d502e9f75a975165f4c86e29167ca8cc2d9d25b5351b46d90d4ab7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='ae690af5ffa639feba3bc04fc804480cdbc40b4099890c9d28dceac8f58f0426'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 10 Jul 2023 21:36:09 GMT
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
	-	`sha256:de858352bd5f94dbc0aec8b677883044449c66a4b3797e1b4110c578929e5611`  
		Last Modified: Mon, 10 Jul 2023 21:43:11 GMT  
		Size: 202.6 MB (202590690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
