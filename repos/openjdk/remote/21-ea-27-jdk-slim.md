## `openjdk:21-ea-27-jdk-slim`

```console
$ docker pull openjdk@sha256:fdb63791d98bdb0f42176b71f279ce4624645700a3d8b1f265c452c11ecce028
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-27-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:9de784252a59485643a96cc43d9cac294ac940028aee2784ed8833942e9db182
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237332718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f23e1a0c44e2b009feec8e0415917d5d643bb6ad857c6d22f3183df03c3b7d4`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:42:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:43:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 18:43:21 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 18:43:21 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jun 2023 01:14:55 GMT
ENV JAVA_VERSION=21-ea+27
# Wed, 21 Jun 2023 01:15:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='686f2ed6faecd9b5be0306df695bafa576758f00efc51b2250a8044a31ddc9af'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6b6f664146527de70f9dcb2d424cf91c6429a41c6e19e9b940819fdfc73aba4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:15:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811e3d95202c7b7a774cb28118272b61b9a762e2b037aa469fd2c653d628bd6`  
		Last Modified: Tue, 13 Jun 2023 18:45:05 GMT  
		Size: 4.0 MB (4007955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edbd202dffa191a8327d2cf2827f6d1694a20a8e19a3c813838103539ac9f1d`  
		Last Modified: Wed, 21 Jun 2023 01:22:27 GMT  
		Size: 204.2 MB (204200019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-27-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3db4cd5e17cdf13a2e2f6d0af1aa323fc250db9dc8bdfc6a8ec6d6bd85699dd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.5 MB (235519632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5764aeac750bef94ec5a07769bc4ea2f91cf15bf562a07461a5f17bdacbf2b`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:27:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:28:10 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 18:28:10 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 18:28:10 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jun 2023 01:15:52 GMT
ENV JAVA_VERSION=21-ea+27
# Wed, 21 Jun 2023 01:16:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='686f2ed6faecd9b5be0306df695bafa576758f00efc51b2250a8044a31ddc9af'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6b6f664146527de70f9dcb2d424cf91c6429a41c6e19e9b940819fdfc73aba4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:16:06 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1887a2e60832f49292b15e0b40386cbefdb18322b6fbb7f3e523b7df6ced1e6e`  
		Last Modified: Tue, 13 Jun 2023 18:29:47 GMT  
		Size: 3.8 MB (3817558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055b5afe28c83da0e6dc967f65bbd493a32c01979f4bc0034073ab2cd932619`  
		Last Modified: Wed, 21 Jun 2023 01:22:50 GMT  
		Size: 202.5 MB (202549540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
