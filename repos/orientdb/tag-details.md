<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `orientdb`

-	[`orientdb:2.0`](#orientdb20)
-	[`orientdb:2.0.18`](#orientdb2018)
-	[`orientdb:2.1`](#orientdb21)
-	[`orientdb:2.1.25`](#orientdb2125)
-	[`orientdb:2.2`](#orientdb22)
-	[`orientdb:2.2.37`](#orientdb2237)
-	[`orientdb:2.2.37-spatial`](#orientdb2237-spatial)
-	[`orientdb:3.0`](#orientdb30)
-	[`orientdb:3.0-tp3`](#orientdb30-tp3)
-	[`orientdb:3.0.38`](#orientdb3038)
-	[`orientdb:3.0.38-tp3`](#orientdb3038-tp3)
-	[`orientdb:3.1`](#orientdb31)
-	[`orientdb:3.1-tp3`](#orientdb31-tp3)
-	[`orientdb:3.1.12`](#orientdb3112)
-	[`orientdb:3.1.12-tp3`](#orientdb3112-tp3)
-	[`orientdb:3.2`](#orientdb32)
-	[`orientdb:3.2-tp3`](#orientdb32-tp3)
-	[`orientdb:3.2.2`](#orientdb322)
-	[`orientdb:3.2.2-tp3`](#orientdb322-tp3)
-	[`orientdb:latest`](#orientdblatest)

## `orientdb:2.0`

```console
$ docker pull orientdb@sha256:f718261da0125e2fe732a5a5baaff018525b3f51bacc059f3eda950563a30363
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:2.0` - linux; amd64

```console
$ docker pull orientdb@sha256:25dad7cf8cb141c55f432227d846296810109742b65e57ce3578c4539e2ab74f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283514255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45ce6a97178e6bf14ebfcf268b9cdcb3b47784a62ea1525fd2c0c6f4dff42080`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:28:10 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:28:10 GMT
ENV ORIENTDB_VERSION=2.0.18
# Wed, 29 Sep 2021 10:28:10 GMT
ENV ORIENTDB_DOWNLOAD_MD5=9e7b7e7b6d95795b188adb4e5898a1b8
# Wed, 29 Sep 2021 10:28:10 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=f562794536bbf8ae2145f96153e58b1e5d9211b3
# Wed, 29 Sep 2021 10:28:16 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:28:16 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:28:16 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:28:17 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:28:17 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:28:17 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:28:17 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19992476c473273ed35d73345aefc6283614d7d52c2cb9b64f484103894f84`  
		Last Modified: Wed, 29 Sep 2021 10:30:45 GMT  
		Size: 46.6 MB (46586572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.0.18`

```console
$ docker pull orientdb@sha256:f718261da0125e2fe732a5a5baaff018525b3f51bacc059f3eda950563a30363
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:2.0.18` - linux; amd64

```console
$ docker pull orientdb@sha256:25dad7cf8cb141c55f432227d846296810109742b65e57ce3578c4539e2ab74f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283514255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45ce6a97178e6bf14ebfcf268b9cdcb3b47784a62ea1525fd2c0c6f4dff42080`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:28:10 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:28:10 GMT
ENV ORIENTDB_VERSION=2.0.18
# Wed, 29 Sep 2021 10:28:10 GMT
ENV ORIENTDB_DOWNLOAD_MD5=9e7b7e7b6d95795b188adb4e5898a1b8
# Wed, 29 Sep 2021 10:28:10 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=f562794536bbf8ae2145f96153e58b1e5d9211b3
# Wed, 29 Sep 2021 10:28:16 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:28:16 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:28:16 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:28:17 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:28:17 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:28:17 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:28:17 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19992476c473273ed35d73345aefc6283614d7d52c2cb9b64f484103894f84`  
		Last Modified: Wed, 29 Sep 2021 10:30:45 GMT  
		Size: 46.6 MB (46586572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.1`

```console
$ docker pull orientdb@sha256:d0cbeb75d5280c2b8d51922da005381991e80c3f88982890dd0d05a992d3dffb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:2.1` - linux; amd64

```console
$ docker pull orientdb@sha256:74c32de59e613e4f46cc97a5cfe7d70e9682d530a962531d0e9bcc1d6f582b83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172403045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d74929419f5cd704f2ef6976bcdf6055f2a9d36a2bda5b6731b73f53a310d9a`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:27:57 GMT
ENV ORIENTDB_VERSION=2.1.25
# Wed, 29 Sep 2021 10:27:57 GMT
ENV ORIENTDB_DOWNLOAD_MD5=054da3fb7c56e7822b2af116966576ce
# Wed, 29 Sep 2021 10:27:57 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=b7b08242b40117ac8eb9a201f8704bde839dfcb8
# Wed, 29 Sep 2021 10:28:02 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:28:05 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:28:05 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:28:05 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:28:05 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:28:06 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:28:06 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:28:06 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0abcf9821f4177d577706bda3f834b3f75f8e79f150523017914db2045a7070a`  
		Last Modified: Wed, 29 Sep 2021 10:30:30 GMT  
		Size: 2.1 MB (2102082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb1cc1b3a550c4f92ea81087af87e7d82bb88aced2ee18e9b3921b17cc3e430`  
		Last Modified: Wed, 29 Sep 2021 10:30:31 GMT  
		Size: 31.1 MB (31087999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.1.25`

```console
$ docker pull orientdb@sha256:d0cbeb75d5280c2b8d51922da005381991e80c3f88982890dd0d05a992d3dffb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:2.1.25` - linux; amd64

```console
$ docker pull orientdb@sha256:74c32de59e613e4f46cc97a5cfe7d70e9682d530a962531d0e9bcc1d6f582b83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172403045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d74929419f5cd704f2ef6976bcdf6055f2a9d36a2bda5b6731b73f53a310d9a`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:27:57 GMT
ENV ORIENTDB_VERSION=2.1.25
# Wed, 29 Sep 2021 10:27:57 GMT
ENV ORIENTDB_DOWNLOAD_MD5=054da3fb7c56e7822b2af116966576ce
# Wed, 29 Sep 2021 10:27:57 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=b7b08242b40117ac8eb9a201f8704bde839dfcb8
# Wed, 29 Sep 2021 10:28:02 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:28:05 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:28:05 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:28:05 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:28:05 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:28:06 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:28:06 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:28:06 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0abcf9821f4177d577706bda3f834b3f75f8e79f150523017914db2045a7070a`  
		Last Modified: Wed, 29 Sep 2021 10:30:30 GMT  
		Size: 2.1 MB (2102082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb1cc1b3a550c4f92ea81087af87e7d82bb88aced2ee18e9b3921b17cc3e430`  
		Last Modified: Wed, 29 Sep 2021 10:30:31 GMT  
		Size: 31.1 MB (31087999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2`

```console
$ docker pull orientdb@sha256:3ecd2ecc20a1d6777406669bae26a14109118c0084208f307991e1f449eb0cb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:2.2` - linux; amd64

```console
$ docker pull orientdb@sha256:e3a041f036e204cef6e3030d94293441271eb512dc9034aeef84c0e7a3b8c8d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187788868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae13433555f1a7fde7cad364b9725a691c4187eee5fdd796ce92a4ec10f822ad`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_VERSION=2.2.37
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Wed, 29 Sep 2021 10:27:40 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Wed, 29 Sep 2021 10:27:44 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:47 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:47 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:48 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:48 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:48 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:48 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:48 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0534e3fb2e5ac80df05c77d5e5bcdb8da109710023126147b6755f5859b154`  
		Last Modified: Wed, 29 Sep 2021 10:30:10 GMT  
		Size: 2.1 MB (2102033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e6575b3495df76c213caba4c001b9c8dddfc8024b9e1a996868391d9f15fb1`  
		Last Modified: Wed, 29 Sep 2021 10:30:13 GMT  
		Size: 46.5 MB (46473871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2.37`

```console
$ docker pull orientdb@sha256:3ecd2ecc20a1d6777406669bae26a14109118c0084208f307991e1f449eb0cb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:2.2.37` - linux; amd64

```console
$ docker pull orientdb@sha256:e3a041f036e204cef6e3030d94293441271eb512dc9034aeef84c0e7a3b8c8d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187788868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae13433555f1a7fde7cad364b9725a691c4187eee5fdd796ce92a4ec10f822ad`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_VERSION=2.2.37
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Wed, 29 Sep 2021 10:27:40 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Wed, 29 Sep 2021 10:27:44 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:47 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:47 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:48 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:48 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:48 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:48 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:48 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0534e3fb2e5ac80df05c77d5e5bcdb8da109710023126147b6755f5859b154`  
		Last Modified: Wed, 29 Sep 2021 10:30:10 GMT  
		Size: 2.1 MB (2102033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e6575b3495df76c213caba4c001b9c8dddfc8024b9e1a996868391d9f15fb1`  
		Last Modified: Wed, 29 Sep 2021 10:30:13 GMT  
		Size: 46.5 MB (46473871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2.37-spatial`

```console
$ docker pull orientdb@sha256:82d0df329f95696802d3fd2a9a43e0b300001fc3fe9d0d37cd92a7c0f91aff43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:2.2.37-spatial` - linux; amd64

```console
$ docker pull orientdb@sha256:1f9203c7ceee14e69867327023c03fc07de7b02ffb8f4b8fec1a40909cccaf3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (188991456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc910fcfe46cf23a4c5579ab8da6ab5aa55f3630dd1c0a8f0e118b2c81ebe6bc`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_VERSION=2.2.37
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Wed, 29 Sep 2021 10:27:39 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Wed, 29 Sep 2021 10:27:40 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Wed, 29 Sep 2021 10:27:44 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:47 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:47 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:48 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:48 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:48 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:48 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:48 GMT
CMD ["server.sh"]
# Wed, 29 Sep 2021 10:27:52 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_MD5=9f64ab5e959f5d9ad9ea5195d6d621d2
# Wed, 29 Sep 2021 10:27:52 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_SHA1=1748c9779ea7a8cb8fc068fcabf960e1778e8a19
# Wed, 29 Sep 2021 10:27:52 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-spatial/2.2.37/orientdb-spatial-2.2.37-dist.jar
# Wed, 29 Sep 2021 10:27:54 GMT
RUN wget $ORIENTDB_DOWNLOAD_SPATIAL_URL     && echo "$ORIENTDB_DOWNLOAD_SPATIAL_MD5 *orientdb-spatial-$ORIENTDB_VERSION-dist.jar" | md5sum -c -     && echo "$ORIENTDB_DOWNLOAD_SPATIAL_SHA1 *orientdb-spatial-$ORIENTDB_VERSION-dist.jar" | sha1sum -c -     && mv orientdb-spatial-*-dist.jar /orientdb/lib/
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0534e3fb2e5ac80df05c77d5e5bcdb8da109710023126147b6755f5859b154`  
		Last Modified: Wed, 29 Sep 2021 10:30:10 GMT  
		Size: 2.1 MB (2102033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e6575b3495df76c213caba4c001b9c8dddfc8024b9e1a996868391d9f15fb1`  
		Last Modified: Wed, 29 Sep 2021 10:30:13 GMT  
		Size: 46.5 MB (46473871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f082dec4d21d40d1a441882b9e3278af4a9a5ab9fb348044a3ee79fa10ad59`  
		Last Modified: Wed, 29 Sep 2021 10:30:23 GMT  
		Size: 1.2 MB (1202588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0`

```console
$ docker pull orientdb@sha256:ca2633f8546664e250daa4a7e1ba29236d1843139ab1a247a5142ae4f9c73a3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.0` - linux; amd64

```console
$ docker pull orientdb@sha256:04a7e464fbbd8aa46c12b6083b24d97322cd80e086a17ffc4786d5856f77c4db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.3 MB (178340030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05410ecaad9f7ccbbc15def9aedd84fc49dc3af71e4086aae65253db71e6993`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:27:10 GMT
ENV ORIENTDB_VERSION=3.0.38
# Wed, 29 Sep 2021 10:27:11 GMT
ENV ORIENTDB_DOWNLOAD_MD5=469b81178b6281db18678be28cf6ebd2
# Wed, 29 Sep 2021 10:27:11 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=e36fc6d6660bfcfb3f938249a13e120a943a35cf
# Wed, 29 Sep 2021 10:27:11 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.0.38/orientdb-community-3.0.38.tar.gz
# Wed, 29 Sep 2021 10:27:15 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:19 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:19 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:20 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:20 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:20 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:20 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:20 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a1350268dd68ad1bdb04b338bfe43ebc1ddef937aa96761d02da35bd088c0c`  
		Last Modified: Wed, 29 Sep 2021 10:29:43 GMT  
		Size: 2.1 MB (2102086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f74e8b0bb99dbc11a1c860367710d7527c7e0c488cf80fd21ef9937551ed3a`  
		Last Modified: Wed, 29 Sep 2021 10:29:45 GMT  
		Size: 37.0 MB (37024980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0-tp3`

```console
$ docker pull orientdb@sha256:0736d34ca00f7ba13fa2adfbb44ec574b4428d4cfa238b1b03d177f4095127a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.0-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:a7ee7c71022ab2234ceec4df3d9954edca1bd9022466489637a1407cd98284f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205360896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b001d7fec24be9931b41f9e1ce7c74fc47abede0e76b50ef2e96857b38bfd566`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:27:10 GMT
ENV ORIENTDB_VERSION=3.0.38
# Wed, 29 Sep 2021 10:27:23 GMT
ENV ORIENTDB_DOWNLOAD_MD5=f851ef569defd1dbaa1fd14def7862f1
# Wed, 29 Sep 2021 10:27:24 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=ec6ffbfc3e99b4fc9f1b57d72dd4e0d40b1e5883
# Wed, 29 Sep 2021 10:27:24 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.0.38/orientdb-tp3-3.0.38.tar.gz
# Wed, 29 Sep 2021 10:27:28 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:34 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:34 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 29 Sep 2021 10:27:34 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:34 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:34 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:35 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:35 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:35 GMT
EXPOSE 8182
# Wed, 29 Sep 2021 10:27:35 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f347f15d1f1f6cdce38b8134c5f1f104717923c93068a52eb2e54f5b4d461fd`  
		Last Modified: Wed, 29 Sep 2021 10:29:55 GMT  
		Size: 2.1 MB (2102110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4f85399d5366f53557079fa119ad57cd30f1bd45d3fa3409f4dcad5d9df21b`  
		Last Modified: Wed, 29 Sep 2021 10:29:59 GMT  
		Size: 64.0 MB (64044446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f5228618d6ebf62a6cfeaf47c92ea53f538dd0b021a90221eae2cc55ea71bc`  
		Last Modified: Wed, 29 Sep 2021 10:29:55 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0.38`

```console
$ docker pull orientdb@sha256:ca2633f8546664e250daa4a7e1ba29236d1843139ab1a247a5142ae4f9c73a3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.0.38` - linux; amd64

```console
$ docker pull orientdb@sha256:04a7e464fbbd8aa46c12b6083b24d97322cd80e086a17ffc4786d5856f77c4db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.3 MB (178340030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05410ecaad9f7ccbbc15def9aedd84fc49dc3af71e4086aae65253db71e6993`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:27:10 GMT
ENV ORIENTDB_VERSION=3.0.38
# Wed, 29 Sep 2021 10:27:11 GMT
ENV ORIENTDB_DOWNLOAD_MD5=469b81178b6281db18678be28cf6ebd2
# Wed, 29 Sep 2021 10:27:11 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=e36fc6d6660bfcfb3f938249a13e120a943a35cf
# Wed, 29 Sep 2021 10:27:11 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.0.38/orientdb-community-3.0.38.tar.gz
# Wed, 29 Sep 2021 10:27:15 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:19 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:19 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:20 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:20 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:20 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:20 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:20 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a1350268dd68ad1bdb04b338bfe43ebc1ddef937aa96761d02da35bd088c0c`  
		Last Modified: Wed, 29 Sep 2021 10:29:43 GMT  
		Size: 2.1 MB (2102086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f74e8b0bb99dbc11a1c860367710d7527c7e0c488cf80fd21ef9937551ed3a`  
		Last Modified: Wed, 29 Sep 2021 10:29:45 GMT  
		Size: 37.0 MB (37024980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0.38-tp3`

```console
$ docker pull orientdb@sha256:0736d34ca00f7ba13fa2adfbb44ec574b4428d4cfa238b1b03d177f4095127a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.0.38-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:a7ee7c71022ab2234ceec4df3d9954edca1bd9022466489637a1407cd98284f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205360896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b001d7fec24be9931b41f9e1ce7c74fc47abede0e76b50ef2e96857b38bfd566`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:27:10 GMT
ENV ORIENTDB_VERSION=3.0.38
# Wed, 29 Sep 2021 10:27:23 GMT
ENV ORIENTDB_DOWNLOAD_MD5=f851ef569defd1dbaa1fd14def7862f1
# Wed, 29 Sep 2021 10:27:24 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=ec6ffbfc3e99b4fc9f1b57d72dd4e0d40b1e5883
# Wed, 29 Sep 2021 10:27:24 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.0.38/orientdb-tp3-3.0.38.tar.gz
# Wed, 29 Sep 2021 10:27:28 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:34 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:34 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 29 Sep 2021 10:27:34 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:34 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:34 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:35 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:35 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:35 GMT
EXPOSE 8182
# Wed, 29 Sep 2021 10:27:35 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f347f15d1f1f6cdce38b8134c5f1f104717923c93068a52eb2e54f5b4d461fd`  
		Last Modified: Wed, 29 Sep 2021 10:29:55 GMT  
		Size: 2.1 MB (2102110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4f85399d5366f53557079fa119ad57cd30f1bd45d3fa3409f4dcad5d9df21b`  
		Last Modified: Wed, 29 Sep 2021 10:29:59 GMT  
		Size: 64.0 MB (64044446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f5228618d6ebf62a6cfeaf47c92ea53f538dd0b021a90221eae2cc55ea71bc`  
		Last Modified: Wed, 29 Sep 2021 10:29:55 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.1`

```console
$ docker pull orientdb@sha256:c5f3e762a3bfdf632a86f1b185ce20b0962a7dc810614ad65c91fe3502822ade
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.1` - linux; amd64

```console
$ docker pull orientdb@sha256:14b69be64a2ee8e0c6e3ce521ca2a35751d0c81c6160e3bb76158ff7b5847d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193775375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c572ea88974b028ea00d1533d84de95e5b6363c3cde6330fb82a10511e7dbf8`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_VERSION=3.1.12
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_DOWNLOAD_MD5=10305af91357051b3b129773ea21cae6
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=2af6a76c78e405d46cada119f22f14400e4a6275
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.1.12/orientdb-community-3.1.12.tar.gz
# Wed, 29 Sep 2021 10:26:47 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:26:51 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:26:51 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:26:51 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:26:51 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:26:51 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:26:52 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:26:52 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5f755883e58986c8437fe4cec7dc48efd0a586388c9e8b7767fddf434ec9e8`  
		Last Modified: Wed, 29 Sep 2021 10:29:17 GMT  
		Size: 2.1 MB (2102077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e520592260b24aff27c4ccd9a99aca89288a24f080a0e01c7196e8000c034`  
		Last Modified: Wed, 29 Sep 2021 10:29:20 GMT  
		Size: 52.5 MB (52460334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.1-tp3`

```console
$ docker pull orientdb@sha256:c475a0b71e23d303a6032ef3a89ed7050a69cb1997410f7c76f79cb8b5aa3c20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.1-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:1d5859aa9da1b39f5f857a8434375d399b4a53582d215c15d094430b7337e6c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217775597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a930fc6c1e9c8d932ff2e1a2d9e2961f78780af5098f2262e9ed68319c08c898`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_VERSION=3.1.12
# Wed, 29 Sep 2021 10:26:55 GMT
ENV ORIENTDB_DOWNLOAD_MD5=269554b2eeebc0963c636a7f57f76e24
# Wed, 29 Sep 2021 10:26:55 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=a9673917f22f5e71e0e1a89ddfdbf6a702828d89
# Wed, 29 Sep 2021 10:26:55 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.1.12/orientdb-tp3-3.1.12.tar.gz
# Wed, 29 Sep 2021 10:27:00 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:04 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:05 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 29 Sep 2021 10:27:05 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:05 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:05 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:06 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:06 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:06 GMT
EXPOSE 8182
# Wed, 29 Sep 2021 10:27:06 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edb0fc9c62b4f7b59018c80a079f9ae9b7062806e425428f298abd02fc4b175`  
		Last Modified: Wed, 29 Sep 2021 10:29:30 GMT  
		Size: 2.1 MB (2102028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee7a5c5515725d25b61269fe2d17115e555ccaaf96dca058b6066e8c8c7e26c`  
		Last Modified: Wed, 29 Sep 2021 10:29:33 GMT  
		Size: 76.5 MB (76459226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47737631b892110ed6e68fbd51586935e28e140a2cf34ec5663ba94d58343af`  
		Last Modified: Wed, 29 Sep 2021 10:29:29 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.1.12`

```console
$ docker pull orientdb@sha256:c5f3e762a3bfdf632a86f1b185ce20b0962a7dc810614ad65c91fe3502822ade
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.1.12` - linux; amd64

```console
$ docker pull orientdb@sha256:14b69be64a2ee8e0c6e3ce521ca2a35751d0c81c6160e3bb76158ff7b5847d8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193775375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c572ea88974b028ea00d1533d84de95e5b6363c3cde6330fb82a10511e7dbf8`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_VERSION=3.1.12
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_DOWNLOAD_MD5=10305af91357051b3b129773ea21cae6
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=2af6a76c78e405d46cada119f22f14400e4a6275
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.1.12/orientdb-community-3.1.12.tar.gz
# Wed, 29 Sep 2021 10:26:47 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:26:51 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:26:51 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:26:51 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:26:51 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:26:51 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:26:52 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:26:52 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5f755883e58986c8437fe4cec7dc48efd0a586388c9e8b7767fddf434ec9e8`  
		Last Modified: Wed, 29 Sep 2021 10:29:17 GMT  
		Size: 2.1 MB (2102077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e520592260b24aff27c4ccd9a99aca89288a24f080a0e01c7196e8000c034`  
		Last Modified: Wed, 29 Sep 2021 10:29:20 GMT  
		Size: 52.5 MB (52460334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.1.12-tp3`

```console
$ docker pull orientdb@sha256:c475a0b71e23d303a6032ef3a89ed7050a69cb1997410f7c76f79cb8b5aa3c20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.1.12-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:1d5859aa9da1b39f5f857a8434375d399b4a53582d215c15d094430b7337e6c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217775597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a930fc6c1e9c8d932ff2e1a2d9e2961f78780af5098f2262e9ed68319c08c898`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:42 GMT
ENV ORIENTDB_VERSION=3.1.12
# Wed, 29 Sep 2021 10:26:55 GMT
ENV ORIENTDB_DOWNLOAD_MD5=269554b2eeebc0963c636a7f57f76e24
# Wed, 29 Sep 2021 10:26:55 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=a9673917f22f5e71e0e1a89ddfdbf6a702828d89
# Wed, 29 Sep 2021 10:26:55 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.1.12/orientdb-tp3-3.1.12.tar.gz
# Wed, 29 Sep 2021 10:27:00 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:27:04 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:27:05 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 29 Sep 2021 10:27:05 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:27:05 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:27:05 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:27:06 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:27:06 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:27:06 GMT
EXPOSE 8182
# Wed, 29 Sep 2021 10:27:06 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edb0fc9c62b4f7b59018c80a079f9ae9b7062806e425428f298abd02fc4b175`  
		Last Modified: Wed, 29 Sep 2021 10:29:30 GMT  
		Size: 2.1 MB (2102028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee7a5c5515725d25b61269fe2d17115e555ccaaf96dca058b6066e8c8c7e26c`  
		Last Modified: Wed, 29 Sep 2021 10:29:33 GMT  
		Size: 76.5 MB (76459226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47737631b892110ed6e68fbd51586935e28e140a2cf34ec5663ba94d58343af`  
		Last Modified: Wed, 29 Sep 2021 10:29:29 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.2`

```console
$ docker pull orientdb@sha256:24204a973478592a6676e9f8bcf7250bd245776d89e7b71b6e6cba93eab578b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.2` - linux; amd64

```console
$ docker pull orientdb@sha256:5db8bb1f48297b1b7f1fe621aa7cfc42f6c878e76e16b4f56fc881cc315e1a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.1 MB (212103143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61dc99720e8e29baf26ac21413073fb5f11f7166369db1f46d59d072a73b2e1d`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_VERSION=3.2.2
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_DOWNLOAD_MD5=623bb47f86503984c401a13d0000979b
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=d167455158bd5c2a009c5631a6b6081136cf482c
# Wed, 29 Sep 2021 10:26:09 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.2.2/orientdb-community-3.2.2.tar.gz
# Wed, 29 Sep 2021 10:26:13 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:26:19 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:26:19 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:26:19 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:26:20 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:26:20 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:26:20 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:26:20 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ec33c23f03b53fcaa1b17334fbd2abfe06e0cb049fc0e430d7f8cc152d463e`  
		Last Modified: Wed, 29 Sep 2021 10:28:44 GMT  
		Size: 2.1 MB (2102083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4debe4fcae474da4a63d13be2ae450ea471eb2f0065db12db8cc7cfbe40592`  
		Last Modified: Wed, 29 Sep 2021 10:28:48 GMT  
		Size: 70.8 MB (70788096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.2-tp3`

```console
$ docker pull orientdb@sha256:a6b5b8d9d925ede16c2589cc370d05072a3feeb13e4043740441a2de20382d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.2-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:3b141a61290f30daa7fbe55c6049e70dd0d6a1733587164cadc382dc4e6026cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.6 MB (248592305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4662db52df3c9244d7ab8add9f9d685164c18a1eb7e10d3d698b14dbe600c64c`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_VERSION=3.2.2
# Wed, 29 Sep 2021 10:26:24 GMT
ENV ORIENTDB_DOWNLOAD_MD5=374a952e2a1dd78306084359aa227831
# Wed, 29 Sep 2021 10:26:24 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=5f566d08e713cea544487257e6c428dd923b017f
# Wed, 29 Sep 2021 10:26:24 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.2.2/orientdb-tp3-3.2.2.tar.gz
# Wed, 29 Sep 2021 10:26:29 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:26:35 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:26:36 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 29 Sep 2021 10:26:36 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:26:36 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:26:36 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:26:37 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:26:37 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:26:37 GMT
EXPOSE 8182
# Wed, 29 Sep 2021 10:26:37 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2508aff59e8955087be0904a38ba4e57b34be4589b6a8f420277a879e85b6b6`  
		Last Modified: Wed, 29 Sep 2021 10:29:01 GMT  
		Size: 2.1 MB (2102085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6f6586f175a31a17e534e53e7faa63c44e9bfecc9dbd2de91a9a0d5cebd764`  
		Last Modified: Wed, 29 Sep 2021 10:29:07 GMT  
		Size: 107.3 MB (107275881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19345531c709b9c7aa26b3b0ff998cc31ba3b7abba7d64fc050d57355e6fb10`  
		Last Modified: Wed, 29 Sep 2021 10:29:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.2.2`

```console
$ docker pull orientdb@sha256:24204a973478592a6676e9f8bcf7250bd245776d89e7b71b6e6cba93eab578b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.2.2` - linux; amd64

```console
$ docker pull orientdb@sha256:5db8bb1f48297b1b7f1fe621aa7cfc42f6c878e76e16b4f56fc881cc315e1a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.1 MB (212103143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61dc99720e8e29baf26ac21413073fb5f11f7166369db1f46d59d072a73b2e1d`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_VERSION=3.2.2
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_DOWNLOAD_MD5=623bb47f86503984c401a13d0000979b
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=d167455158bd5c2a009c5631a6b6081136cf482c
# Wed, 29 Sep 2021 10:26:09 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.2.2/orientdb-community-3.2.2.tar.gz
# Wed, 29 Sep 2021 10:26:13 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:26:19 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:26:19 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:26:19 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:26:20 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:26:20 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:26:20 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:26:20 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ec33c23f03b53fcaa1b17334fbd2abfe06e0cb049fc0e430d7f8cc152d463e`  
		Last Modified: Wed, 29 Sep 2021 10:28:44 GMT  
		Size: 2.1 MB (2102083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4debe4fcae474da4a63d13be2ae450ea471eb2f0065db12db8cc7cfbe40592`  
		Last Modified: Wed, 29 Sep 2021 10:28:48 GMT  
		Size: 70.8 MB (70788096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.2.2-tp3`

```console
$ docker pull orientdb@sha256:a6b5b8d9d925ede16c2589cc370d05072a3feeb13e4043740441a2de20382d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:3.2.2-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:3b141a61290f30daa7fbe55c6049e70dd0d6a1733587164cadc382dc4e6026cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.6 MB (248592305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4662db52df3c9244d7ab8add9f9d685164c18a1eb7e10d3d698b14dbe600c64c`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_VERSION=3.2.2
# Wed, 29 Sep 2021 10:26:24 GMT
ENV ORIENTDB_DOWNLOAD_MD5=374a952e2a1dd78306084359aa227831
# Wed, 29 Sep 2021 10:26:24 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=5f566d08e713cea544487257e6c428dd923b017f
# Wed, 29 Sep 2021 10:26:24 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.2.2/orientdb-tp3-3.2.2.tar.gz
# Wed, 29 Sep 2021 10:26:29 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:26:35 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:26:36 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 29 Sep 2021 10:26:36 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:26:36 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:26:36 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:26:37 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:26:37 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:26:37 GMT
EXPOSE 8182
# Wed, 29 Sep 2021 10:26:37 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2508aff59e8955087be0904a38ba4e57b34be4589b6a8f420277a879e85b6b6`  
		Last Modified: Wed, 29 Sep 2021 10:29:01 GMT  
		Size: 2.1 MB (2102085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6f6586f175a31a17e534e53e7faa63c44e9bfecc9dbd2de91a9a0d5cebd764`  
		Last Modified: Wed, 29 Sep 2021 10:29:07 GMT  
		Size: 107.3 MB (107275881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19345531c709b9c7aa26b3b0ff998cc31ba3b7abba7d64fc050d57355e6fb10`  
		Last Modified: Wed, 29 Sep 2021 10:29:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:latest`

```console
$ docker pull orientdb@sha256:24204a973478592a6676e9f8bcf7250bd245776d89e7b71b6e6cba93eab578b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:latest` - linux; amd64

```console
$ docker pull orientdb@sha256:5db8bb1f48297b1b7f1fe621aa7cfc42f6c878e76e16b4f56fc881cc315e1a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.1 MB (212103143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61dc99720e8e29baf26ac21413073fb5f11f7166369db1f46d59d072a73b2e1d`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:25:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:25:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:25:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:25:13 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:25:13 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 10:26:08 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 29 Sep 2021 10:26:08 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_VERSION=3.2.2
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_DOWNLOAD_MD5=623bb47f86503984c401a13d0000979b
# Wed, 29 Sep 2021 10:26:08 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=d167455158bd5c2a009c5631a6b6081136cf482c
# Wed, 29 Sep 2021 10:26:09 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.2.2/orientdb-community-3.2.2.tar.gz
# Wed, 29 Sep 2021 10:26:13 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 10:26:19 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 29 Sep 2021 10:26:19 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:26:19 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 29 Sep 2021 10:26:20 GMT
WORKDIR /orientdb
# Wed, 29 Sep 2021 10:26:20 GMT
EXPOSE 2424
# Wed, 29 Sep 2021 10:26:20 GMT
EXPOSE 2480
# Wed, 29 Sep 2021 10:26:20 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb783f109fe5199148a46daa8c799d3bde27b23584ee8db6f225a1a7aa6469`  
		Last Modified: Tue, 28 Sep 2021 09:47:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee21827af058c437be414e384a26dd7f0ac195258c020a857c17e9fdb87c9d`  
		Last Modified: Tue, 28 Sep 2021 09:47:19 GMT  
		Size: 106.3 MB (106261825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ec33c23f03b53fcaa1b17334fbd2abfe06e0cb049fc0e430d7f8cc152d463e`  
		Last Modified: Wed, 29 Sep 2021 10:28:44 GMT  
		Size: 2.1 MB (2102083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4debe4fcae474da4a63d13be2ae450ea471eb2f0065db12db8cc7cfbe40592`  
		Last Modified: Wed, 29 Sep 2021 10:28:48 GMT  
		Size: 70.8 MB (70788096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
