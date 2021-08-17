## `orientdb:latest`

```console
$ docker pull orientdb@sha256:e244f5f9574915efbcace2fd68a42f1ab0f3ae6fdf4e0debdcea44398b196d01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:latest` - linux; amd64

```console
$ docker pull orientdb@sha256:8fa2d847a6c54eeafc8cf200e7706adda8874c00d010a3be57273bbefaf0b00a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.5 MB (209523905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c4a8d5625a5aac3b66ea76ff90514f096150a6af2052f48ce15907693c8cca`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:55:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 17 Aug 2021 06:55:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:55:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:55:47 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:55:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 17 Aug 2021 06:56:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 17 Aug 2021 20:29:11 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Tue, 17 Aug 2021 20:29:12 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Tue, 17 Aug 2021 20:29:12 GMT
ENV ORIENTDB_VERSION=3.2.0
# Tue, 17 Aug 2021 20:29:12 GMT
ENV ORIENTDB_DOWNLOAD_MD5=7bff911bea6b02d2f1d9ddff5e4ba8ea
# Tue, 17 Aug 2021 20:29:12 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=f424731e3d078de692fab97d6aa3b3e8395d7d01
# Tue, 17 Aug 2021 20:29:12 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.2.0/orientdb-community-3.2.0.tar.gz
# Tue, 17 Aug 2021 20:29:19 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:29:25 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Tue, 17 Aug 2021 20:29:25 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 20:29:26 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Tue, 17 Aug 2021 20:29:26 GMT
WORKDIR /orientdb
# Tue, 17 Aug 2021 20:29:26 GMT
EXPOSE 2424
# Tue, 17 Aug 2021 20:29:26 GMT
EXPOSE 2480
# Tue, 17 Aug 2021 20:29:27 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d3ca35fb9a4f8f161dc8b1007db271091ce462aa5a6c8aada7e7096f9857b5`  
		Last Modified: Tue, 17 Aug 2021 07:04:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fdd77aee065a3593352d4910487a661d9f1cc12555573e767f55ba3e1c10e0`  
		Last Modified: Tue, 17 Aug 2021 07:04:19 GMT  
		Size: 106.3 MB (106270512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf2349de1b0a336f16a0bf37762308c537e5a651cac715495ce1a5259040e78`  
		Last Modified: Tue, 17 Aug 2021 20:32:10 GMT  
		Size: 2.6 MB (2615958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4714ba24fc52f5659eacd6615d45d2907de296aae9db6f248614d885a16450b5`  
		Last Modified: Tue, 17 Aug 2021 20:32:14 GMT  
		Size: 70.2 MB (70222471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
