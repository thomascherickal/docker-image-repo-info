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
-	[`orientdb:3.0.33`](#orientdb3033)
-	[`orientdb:3.0.33-tp3`](#orientdb3033-tp3)
-	[`orientdb:3.0-tp3`](#orientdb30-tp3)
-	[`orientdb:3.1`](#orientdb31)
-	[`orientdb:3.1.1`](#orientdb311)
-	[`orientdb:3.1.1-tp3`](#orientdb311-tp3)
-	[`orientdb:3.1-tp3`](#orientdb31-tp3)
-	[`orientdb:latest`](#orientdblatest)

## `orientdb:2.0`

```console
$ docker pull orientdb@sha256:4dd68916ceef94f2617a3c7ebf1ebef93b0d6ad886abbe7416535e09c59f0cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.0` - linux; amd64

```console
$ docker pull orientdb@sha256:c4c3f8f4a3f4f82bad3af5f75ac0ad8a019c4fa742fe00995cdd41c9acec4dd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.7 MB (276746900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe4859f45d41a4d68d455ee6491e8112cb922c1d1c300ea00272827cb880271`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:44:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:44:26 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:47 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:45:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:45:48 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:45:55 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:03:59 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:04:00 GMT
ENV ORIENTDB_VERSION=2.0.18
# Wed, 05 Aug 2020 18:04:00 GMT
ENV ORIENTDB_DOWNLOAD_MD5=9e7b7e7b6d95795b188adb4e5898a1b8
# Wed, 05 Aug 2020 18:04:00 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=f562794536bbf8ae2145f96153e58b1e5d9211b3
# Wed, 05 Aug 2020 18:04:04 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:04:04 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:04:04 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:04:04 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:04:04 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:04:05 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:04:05 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf04b6bbed0c757411bf5f2a3e4c76bf09b5527db6b50e326ba99ead51b20fb6`  
		Last Modified: Wed, 05 Aug 2020 00:50:58 GMT  
		Size: 5.3 MB (5284648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41dc8052672fcfe6881aa19d6d70203f3d9baf4ea4ef867834b3aa05102c3821`  
		Last Modified: Wed, 05 Aug 2020 00:52:12 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc65a7534c9a4a591026f53cb17ead091ae2e67df031c1b58ea030bef5bf75`  
		Last Modified: Wed, 05 Aug 2020 00:52:23 GMT  
		Size: 104.8 MB (104841774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97d44c4235f603601509ff5cdc4934fdf33864ee89dac995c65121729a8c22c`  
		Last Modified: Wed, 05 Aug 2020 18:05:28 GMT  
		Size: 46.6 MB (46586534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.0.18`

```console
$ docker pull orientdb@sha256:4dd68916ceef94f2617a3c7ebf1ebef93b0d6ad886abbe7416535e09c59f0cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.0.18` - linux; amd64

```console
$ docker pull orientdb@sha256:c4c3f8f4a3f4f82bad3af5f75ac0ad8a019c4fa742fe00995cdd41c9acec4dd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.7 MB (276746900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe4859f45d41a4d68d455ee6491e8112cb922c1d1c300ea00272827cb880271`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:44:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:44:26 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:47 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:45:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:45:48 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:45:55 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:03:59 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:04:00 GMT
ENV ORIENTDB_VERSION=2.0.18
# Wed, 05 Aug 2020 18:04:00 GMT
ENV ORIENTDB_DOWNLOAD_MD5=9e7b7e7b6d95795b188adb4e5898a1b8
# Wed, 05 Aug 2020 18:04:00 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=f562794536bbf8ae2145f96153e58b1e5d9211b3
# Wed, 05 Aug 2020 18:04:04 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:04:04 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:04:04 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:04:04 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:04:04 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:04:05 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:04:05 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf04b6bbed0c757411bf5f2a3e4c76bf09b5527db6b50e326ba99ead51b20fb6`  
		Last Modified: Wed, 05 Aug 2020 00:50:58 GMT  
		Size: 5.3 MB (5284648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41dc8052672fcfe6881aa19d6d70203f3d9baf4ea4ef867834b3aa05102c3821`  
		Last Modified: Wed, 05 Aug 2020 00:52:12 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc65a7534c9a4a591026f53cb17ead091ae2e67df031c1b58ea030bef5bf75`  
		Last Modified: Wed, 05 Aug 2020 00:52:23 GMT  
		Size: 104.8 MB (104841774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97d44c4235f603601509ff5cdc4934fdf33864ee89dac995c65121729a8c22c`  
		Last Modified: Wed, 05 Aug 2020 18:05:28 GMT  
		Size: 46.6 MB (46586534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.1`

```console
$ docker pull orientdb@sha256:eef28bf7591ec9f2a8428d22218de3348c30fe28b7bc4e6c6b3bbff538ae105c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.1` - linux; amd64

```console
$ docker pull orientdb@sha256:9e22d0a72e9ccd1d19d76ce75cdb1dd688515db67a65fec8403d30e90ae1698a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.2 MB (169154825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042467a9762b184dd89a5012c0004383fcecb45f00c9c1b0d8edac205dba895c`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:03:43 GMT
ENV ORIENTDB_VERSION=2.1.25
# Wed, 05 Aug 2020 18:03:43 GMT
ENV ORIENTDB_DOWNLOAD_MD5=054da3fb7c56e7822b2af116966576ce
# Wed, 05 Aug 2020 18:03:44 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=b7b08242b40117ac8eb9a201f8704bde839dfcb8
# Wed, 05 Aug 2020 18:03:49 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:03:53 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:03:53 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:03:53 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:03:54 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:03:54 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:03:54 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:03:54 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a3777046eeb076ba4a59bf63e386182b72ef6ca01e22eea336d52a048f7925`  
		Last Modified: Wed, 05 Aug 2020 18:05:15 GMT  
		Size: 2.6 MB (2614618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f1cc9f45ac2423a5e9deadf9df4ae0e0490a27e19d9c018382f122d84d1a3`  
		Last Modified: Wed, 05 Aug 2020 18:05:19 GMT  
		Size: 31.1 MB (31087950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.1.25`

```console
$ docker pull orientdb@sha256:eef28bf7591ec9f2a8428d22218de3348c30fe28b7bc4e6c6b3bbff538ae105c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.1.25` - linux; amd64

```console
$ docker pull orientdb@sha256:9e22d0a72e9ccd1d19d76ce75cdb1dd688515db67a65fec8403d30e90ae1698a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.2 MB (169154825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042467a9762b184dd89a5012c0004383fcecb45f00c9c1b0d8edac205dba895c`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:03:43 GMT
ENV ORIENTDB_VERSION=2.1.25
# Wed, 05 Aug 2020 18:03:43 GMT
ENV ORIENTDB_DOWNLOAD_MD5=054da3fb7c56e7822b2af116966576ce
# Wed, 05 Aug 2020 18:03:44 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=b7b08242b40117ac8eb9a201f8704bde839dfcb8
# Wed, 05 Aug 2020 18:03:49 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:03:53 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:03:53 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:03:53 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:03:54 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:03:54 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:03:54 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:03:54 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a3777046eeb076ba4a59bf63e386182b72ef6ca01e22eea336d52a048f7925`  
		Last Modified: Wed, 05 Aug 2020 18:05:15 GMT  
		Size: 2.6 MB (2614618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f1cc9f45ac2423a5e9deadf9df4ae0e0490a27e19d9c018382f122d84d1a3`  
		Last Modified: Wed, 05 Aug 2020 18:05:19 GMT  
		Size: 31.1 MB (31087950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2`

```console
$ docker pull orientdb@sha256:ce860d65e7c24802ffcedc27d661fc63cc13b10d4e600b7a5328f554b98eeb62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.2` - linux; amd64

```console
$ docker pull orientdb@sha256:211c6e8cd5cded38362b979183f047c29affd84ff0b3800a1a04d8a5816f15e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.5 MB (184540798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4024e18f1aa1df149bc88f7f3b19c3d95c374d310e785e32a219a23b4a002ed`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_VERSION=2.2.37
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Wed, 05 Aug 2020 18:03:30 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:03:33 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:03:33 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:03:33 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:03:33 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:03:33 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:03:34 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:03:34 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb0a23535f095f3ef6d6db68827b121e11e826ee6c20790ad907c80eff5041f`  
		Last Modified: Wed, 05 Aug 2020 18:04:58 GMT  
		Size: 2.6 MB (2614621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48607567f6df7dee24a40b1736a74060df4b4f258b46c6a553bd0574e95e72a`  
		Last Modified: Wed, 05 Aug 2020 18:05:07 GMT  
		Size: 46.5 MB (46473920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2.37`

```console
$ docker pull orientdb@sha256:ce860d65e7c24802ffcedc27d661fc63cc13b10d4e600b7a5328f554b98eeb62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.2.37` - linux; amd64

```console
$ docker pull orientdb@sha256:211c6e8cd5cded38362b979183f047c29affd84ff0b3800a1a04d8a5816f15e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.5 MB (184540798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4024e18f1aa1df149bc88f7f3b19c3d95c374d310e785e32a219a23b4a002ed`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_VERSION=2.2.37
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Wed, 05 Aug 2020 18:03:30 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:03:33 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:03:33 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:03:33 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:03:33 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:03:33 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:03:34 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:03:34 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb0a23535f095f3ef6d6db68827b121e11e826ee6c20790ad907c80eff5041f`  
		Last Modified: Wed, 05 Aug 2020 18:04:58 GMT  
		Size: 2.6 MB (2614621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48607567f6df7dee24a40b1736a74060df4b4f258b46c6a553bd0574e95e72a`  
		Last Modified: Wed, 05 Aug 2020 18:05:07 GMT  
		Size: 46.5 MB (46473920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2.37-spatial`

```console
$ docker pull orientdb@sha256:8fb346eb99afa5c32bb1c78dd598f53b60e4682dffff8d38b20f60106ae369ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.2.37-spatial` - linux; amd64

```console
$ docker pull orientdb@sha256:81f34c26bed2e1e2d4034ac744959f2d7320f908c7693408d568fba9bbe3c182
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.7 MB (185743379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fbfcda8e679ae26194f71d51be87e6f9e705dd975ab209423b174a32ea14cca`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_VERSION=2.2.37
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Wed, 05 Aug 2020 18:03:24 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Wed, 05 Aug 2020 18:03:30 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:03:33 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:03:33 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:03:33 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:03:33 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:03:33 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:03:34 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:03:34 GMT
CMD ["server.sh"]
# Wed, 05 Aug 2020 18:03:38 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_MD5=9f64ab5e959f5d9ad9ea5195d6d621d2
# Wed, 05 Aug 2020 18:03:38 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_SHA1=1748c9779ea7a8cb8fc068fcabf960e1778e8a19
# Wed, 05 Aug 2020 18:03:38 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-spatial/2.2.37/orientdb-spatial-2.2.37-dist.jar
# Wed, 05 Aug 2020 18:03:39 GMT
RUN wget $ORIENTDB_DOWNLOAD_SPATIAL_URL     && echo "$ORIENTDB_DOWNLOAD_SPATIAL_MD5 *orientdb-spatial-$ORIENTDB_VERSION-dist.jar" | md5sum -c -     && echo "$ORIENTDB_DOWNLOAD_SPATIAL_SHA1 *orientdb-spatial-$ORIENTDB_VERSION-dist.jar" | sha1sum -c -     && mv orientdb-spatial-*-dist.jar /orientdb/lib/
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb0a23535f095f3ef6d6db68827b121e11e826ee6c20790ad907c80eff5041f`  
		Last Modified: Wed, 05 Aug 2020 18:04:58 GMT  
		Size: 2.6 MB (2614621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48607567f6df7dee24a40b1736a74060df4b4f258b46c6a553bd0574e95e72a`  
		Last Modified: Wed, 05 Aug 2020 18:05:07 GMT  
		Size: 46.5 MB (46473920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77903bce3bb427322179c21f586b03ab37a56da74b3cfded1f54fda92f3ce3cf`  
		Last Modified: Wed, 05 Aug 2020 18:05:12 GMT  
		Size: 1.2 MB (1202581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0`

```console
$ docker pull orientdb@sha256:71d50d2e2b6f3e4d86403c0db523b54c6cfdf489b52acd673e2abf71f41cd030
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.0` - linux; amd64

```console
$ docker pull orientdb@sha256:53f2b23bd1d89af76d87eaedc9317f1ab72d239356257c15537cc967292fbcc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175075150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0cd594731c478d59c06da4bc43674cdba3d54300318ab94620ab57a0bd6fe2`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 12 Aug 2020 18:22:06 GMT
ENV ORIENTDB_VERSION=3.0.33
# Wed, 12 Aug 2020 18:22:06 GMT
ENV ORIENTDB_DOWNLOAD_MD5=ec89e79a21bd9bf9bec89ba97b2fa7b1
# Wed, 12 Aug 2020 18:22:07 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=2b11b01516424d3452397daeaea393e5de9435c9
# Wed, 12 Aug 2020 18:22:07 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.0.33/orientdb-community-3.0.33.tar.gz
# Wed, 12 Aug 2020 18:22:13 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 18:22:16 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 12 Aug 2020 18:22:16 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 18:22:16 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 12 Aug 2020 18:22:16 GMT
WORKDIR /orientdb
# Wed, 12 Aug 2020 18:22:17 GMT
EXPOSE 2424
# Wed, 12 Aug 2020 18:22:17 GMT
EXPOSE 2480
# Wed, 12 Aug 2020 18:22:17 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439751cfdecbe783cc58997c3533b227f07552679721579fd1efbbc28f34c990`  
		Last Modified: Wed, 12 Aug 2020 18:23:05 GMT  
		Size: 2.6 MB (2614608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73bde47ef8957ced8fad973d649dd5ef8ef9c4a688f8667e2fcad7523cc7b93`  
		Last Modified: Wed, 12 Aug 2020 18:23:09 GMT  
		Size: 37.0 MB (37008285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0.33`

```console
$ docker pull orientdb@sha256:71d50d2e2b6f3e4d86403c0db523b54c6cfdf489b52acd673e2abf71f41cd030
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.0.33` - linux; amd64

```console
$ docker pull orientdb@sha256:53f2b23bd1d89af76d87eaedc9317f1ab72d239356257c15537cc967292fbcc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175075150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0cd594731c478d59c06da4bc43674cdba3d54300318ab94620ab57a0bd6fe2`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 12 Aug 2020 18:22:06 GMT
ENV ORIENTDB_VERSION=3.0.33
# Wed, 12 Aug 2020 18:22:06 GMT
ENV ORIENTDB_DOWNLOAD_MD5=ec89e79a21bd9bf9bec89ba97b2fa7b1
# Wed, 12 Aug 2020 18:22:07 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=2b11b01516424d3452397daeaea393e5de9435c9
# Wed, 12 Aug 2020 18:22:07 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.0.33/orientdb-community-3.0.33.tar.gz
# Wed, 12 Aug 2020 18:22:13 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 18:22:16 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 12 Aug 2020 18:22:16 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 18:22:16 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 12 Aug 2020 18:22:16 GMT
WORKDIR /orientdb
# Wed, 12 Aug 2020 18:22:17 GMT
EXPOSE 2424
# Wed, 12 Aug 2020 18:22:17 GMT
EXPOSE 2480
# Wed, 12 Aug 2020 18:22:17 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439751cfdecbe783cc58997c3533b227f07552679721579fd1efbbc28f34c990`  
		Last Modified: Wed, 12 Aug 2020 18:23:05 GMT  
		Size: 2.6 MB (2614608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73bde47ef8957ced8fad973d649dd5ef8ef9c4a688f8667e2fcad7523cc7b93`  
		Last Modified: Wed, 12 Aug 2020 18:23:09 GMT  
		Size: 37.0 MB (37008285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0.33-tp3`

```console
$ docker pull orientdb@sha256:28c28bfe4a7c937ae2af8ffd5cabea537eecb6359036e377f09ad77f72395720
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.0.33-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:f2497223c51ae30da2213cffdf5df8986cf555a204d9c86575d1d2f5c301507e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202095424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a835031d5039d61973e9ce098794a127cc9d16097e738097532b3decbf4c34`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 12 Aug 2020 18:22:06 GMT
ENV ORIENTDB_VERSION=3.0.33
# Wed, 12 Aug 2020 18:22:23 GMT
ENV ORIENTDB_DOWNLOAD_MD5=e0a30641d5c4a20a36c935d2b0de3c2c
# Wed, 12 Aug 2020 18:22:23 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=71f8a96ed09b7a10931959bdd7567d2653a6095f
# Wed, 12 Aug 2020 18:22:23 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.0.33/orientdb-tp3-3.0.33.tar.gz
# Wed, 12 Aug 2020 18:22:29 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 18:22:35 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 12 Aug 2020 18:22:35 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 12 Aug 2020 18:22:35 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 18:22:35 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 12 Aug 2020 18:22:35 GMT
WORKDIR /orientdb
# Wed, 12 Aug 2020 18:22:36 GMT
EXPOSE 2424
# Wed, 12 Aug 2020 18:22:36 GMT
EXPOSE 2480
# Wed, 12 Aug 2020 18:22:36 GMT
EXPOSE 8182
# Wed, 12 Aug 2020 18:22:36 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebabbc8101f8aff466c6cd37d72c29057bca8a249a4368a28b9adbe68e7b0e98`  
		Last Modified: Wed, 12 Aug 2020 18:23:14 GMT  
		Size: 2.6 MB (2614614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694d9fffd4f9b671c6d9ae2f8ed58ebcd32776f204ff2463a7726090a6609d0d`  
		Last Modified: Wed, 12 Aug 2020 18:23:22 GMT  
		Size: 64.0 MB (64027178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4515e9c66dcd8c9e12854659a026aca9499901cce5c43be51b7d166d969fdc3`  
		Last Modified: Wed, 12 Aug 2020 18:23:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0-tp3`

```console
$ docker pull orientdb@sha256:28c28bfe4a7c937ae2af8ffd5cabea537eecb6359036e377f09ad77f72395720
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.0-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:f2497223c51ae30da2213cffdf5df8986cf555a204d9c86575d1d2f5c301507e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202095424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a835031d5039d61973e9ce098794a127cc9d16097e738097532b3decbf4c34`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 12 Aug 2020 18:22:06 GMT
ENV ORIENTDB_VERSION=3.0.33
# Wed, 12 Aug 2020 18:22:23 GMT
ENV ORIENTDB_DOWNLOAD_MD5=e0a30641d5c4a20a36c935d2b0de3c2c
# Wed, 12 Aug 2020 18:22:23 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=71f8a96ed09b7a10931959bdd7567d2653a6095f
# Wed, 12 Aug 2020 18:22:23 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.0.33/orientdb-tp3-3.0.33.tar.gz
# Wed, 12 Aug 2020 18:22:29 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 18:22:35 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 12 Aug 2020 18:22:35 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 12 Aug 2020 18:22:35 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 18:22:35 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 12 Aug 2020 18:22:35 GMT
WORKDIR /orientdb
# Wed, 12 Aug 2020 18:22:36 GMT
EXPOSE 2424
# Wed, 12 Aug 2020 18:22:36 GMT
EXPOSE 2480
# Wed, 12 Aug 2020 18:22:36 GMT
EXPOSE 8182
# Wed, 12 Aug 2020 18:22:36 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebabbc8101f8aff466c6cd37d72c29057bca8a249a4368a28b9adbe68e7b0e98`  
		Last Modified: Wed, 12 Aug 2020 18:23:14 GMT  
		Size: 2.6 MB (2614614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694d9fffd4f9b671c6d9ae2f8ed58ebcd32776f204ff2463a7726090a6609d0d`  
		Last Modified: Wed, 12 Aug 2020 18:23:22 GMT  
		Size: 64.0 MB (64027178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4515e9c66dcd8c9e12854659a026aca9499901cce5c43be51b7d166d969fdc3`  
		Last Modified: Wed, 12 Aug 2020 18:23:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.1`

```console
$ docker pull orientdb@sha256:081b7cfe3008ed439c53d15eaba0fdad94a3367c2f137ae2c441c3a84ea042f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.1` - linux; amd64

```console
$ docker pull orientdb@sha256:bb0f2427f58ce2dfde12d4ded2c1736ce3ca711d94f6306f7d4393d77ed02ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.4 MB (188444383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1d1e94b436ac91276992c6d04ea36737d5ada52bf2f575d7c44b288b0a62205`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_VERSION=3.1.1
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_MD5=d4576a49cbb1e1a5933761441c762118
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=e874f46aaa62b66721ed924067c49dd759069517
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.1.1/orientdb-community-3.1.1.tar.gz
# Wed, 05 Aug 2020 18:02:25 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:02:29 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:02:29 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:02:29 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:02:29 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:02:29 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:02:30 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:02:30 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fc77ba54e521f28a91f70abb568a9a969bd6d4915d44e3a1e48d31610fedde`  
		Last Modified: Wed, 05 Aug 2020 18:04:15 GMT  
		Size: 2.6 MB (2614631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154095cd463e8d4303cbe6a969ca45487597d6eb231391a2e083de6f99da2335`  
		Last Modified: Wed, 05 Aug 2020 18:04:19 GMT  
		Size: 50.4 MB (50377495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.1.1`

```console
$ docker pull orientdb@sha256:081b7cfe3008ed439c53d15eaba0fdad94a3367c2f137ae2c441c3a84ea042f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.1.1` - linux; amd64

```console
$ docker pull orientdb@sha256:bb0f2427f58ce2dfde12d4ded2c1736ce3ca711d94f6306f7d4393d77ed02ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.4 MB (188444383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1d1e94b436ac91276992c6d04ea36737d5ada52bf2f575d7c44b288b0a62205`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_VERSION=3.1.1
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_MD5=d4576a49cbb1e1a5933761441c762118
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=e874f46aaa62b66721ed924067c49dd759069517
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.1.1/orientdb-community-3.1.1.tar.gz
# Wed, 05 Aug 2020 18:02:25 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:02:29 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:02:29 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:02:29 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:02:29 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:02:29 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:02:30 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:02:30 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fc77ba54e521f28a91f70abb568a9a969bd6d4915d44e3a1e48d31610fedde`  
		Last Modified: Wed, 05 Aug 2020 18:04:15 GMT  
		Size: 2.6 MB (2614631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154095cd463e8d4303cbe6a969ca45487597d6eb231391a2e083de6f99da2335`  
		Last Modified: Wed, 05 Aug 2020 18:04:19 GMT  
		Size: 50.4 MB (50377495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.1.1-tp3`

```console
$ docker pull orientdb@sha256:ac7a2ddd2a713b15f7f75c93e215173692a5ac867493a38bed455d223f2c4e4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.1.1-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:be9a02657fee075f28ebc53c9e4869594cfa3a9e5289e8fa8817d8d5dbcdb33b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212444812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629de379fe75155476bc30dfc572198d5601216fb2d8eb2f47679f655e77a6e6`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_VERSION=3.1.1
# Wed, 05 Aug 2020 18:02:35 GMT
ENV ORIENTDB_DOWNLOAD_MD5=81f24b4926634024cbe63239dfc31dce
# Wed, 05 Aug 2020 18:02:35 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=da9389bdb50d0905e32907e40f050d964686ce47
# Wed, 05 Aug 2020 18:02:35 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.1.1/orientdb-tp3-3.1.1.tar.gz
# Wed, 05 Aug 2020 18:02:41 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:02:46 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:02:46 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 05 Aug 2020 18:02:46 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:02:46 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:02:47 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:02:47 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:02:47 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:02:47 GMT
EXPOSE 8182
# Wed, 05 Aug 2020 18:02:48 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6216bdd1f85a1cd40392975d1a275b1b077f16d38c16814b44e5ad57667162d9`  
		Last Modified: Wed, 05 Aug 2020 18:04:24 GMT  
		Size: 2.6 MB (2614619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3464fb537966e5d5db3d2a6e0212b23f45c68a6629ccd08276643556650fff`  
		Last Modified: Wed, 05 Aug 2020 18:04:31 GMT  
		Size: 74.4 MB (74376560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a8e710d6044c0ac45b9faca3d8efa0efb3a9b75475edae605366dc540a6cdd`  
		Last Modified: Wed, 05 Aug 2020 18:04:24 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.1-tp3`

```console
$ docker pull orientdb@sha256:ac7a2ddd2a713b15f7f75c93e215173692a5ac867493a38bed455d223f2c4e4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.1-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:be9a02657fee075f28ebc53c9e4869594cfa3a9e5289e8fa8817d8d5dbcdb33b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212444812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629de379fe75155476bc30dfc572198d5601216fb2d8eb2f47679f655e77a6e6`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_VERSION=3.1.1
# Wed, 05 Aug 2020 18:02:35 GMT
ENV ORIENTDB_DOWNLOAD_MD5=81f24b4926634024cbe63239dfc31dce
# Wed, 05 Aug 2020 18:02:35 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=da9389bdb50d0905e32907e40f050d964686ce47
# Wed, 05 Aug 2020 18:02:35 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.1.1/orientdb-tp3-3.1.1.tar.gz
# Wed, 05 Aug 2020 18:02:41 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:02:46 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:02:46 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Wed, 05 Aug 2020 18:02:46 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:02:46 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:02:47 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:02:47 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:02:47 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:02:47 GMT
EXPOSE 8182
# Wed, 05 Aug 2020 18:02:48 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6216bdd1f85a1cd40392975d1a275b1b077f16d38c16814b44e5ad57667162d9`  
		Last Modified: Wed, 05 Aug 2020 18:04:24 GMT  
		Size: 2.6 MB (2614619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3464fb537966e5d5db3d2a6e0212b23f45c68a6629ccd08276643556650fff`  
		Last Modified: Wed, 05 Aug 2020 18:04:31 GMT  
		Size: 74.4 MB (74376560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a8e710d6044c0ac45b9faca3d8efa0efb3a9b75475edae605366dc540a6cdd`  
		Last Modified: Wed, 05 Aug 2020 18:04:24 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:latest`

```console
$ docker pull orientdb@sha256:081b7cfe3008ed439c53d15eaba0fdad94a3367c2f137ae2c441c3a84ea042f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:latest` - linux; amd64

```console
$ docker pull orientdb@sha256:bb0f2427f58ce2dfde12d4ded2c1736ce3ca711d94f6306f7d4393d77ed02ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.4 MB (188444383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1d1e94b436ac91276992c6d04ea36737d5ada52bf2f575d7c44b288b0a62205`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 05 Aug 2020 00:45:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:46:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:46:00 GMT
ENV JAVA_VERSION=8u265
# Wed, 05 Aug 2020 00:46:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 05 Aug 2020 18:02:18 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 05 Aug 2020 18:02:19 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_VERSION=3.1.1
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_MD5=d4576a49cbb1e1a5933761441c762118
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=e874f46aaa62b66721ed924067c49dd759069517
# Wed, 05 Aug 2020 18:02:19 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.1.1/orientdb-community-3.1.1.tar.gz
# Wed, 05 Aug 2020 18:02:25 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 18:02:29 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 05 Aug 2020 18:02:29 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 18:02:29 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 05 Aug 2020 18:02:29 GMT
WORKDIR /orientdb
# Wed, 05 Aug 2020 18:02:29 GMT
EXPOSE 2424
# Wed, 05 Aug 2020 18:02:30 GMT
EXPOSE 2480
# Wed, 05 Aug 2020 18:02:30 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b86d6fc625bd29e1581869da80f01a1516aabbc3fb1795a72d81bc8ff8d3e`  
		Last Modified: Wed, 05 Aug 2020 00:52:28 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef007d5ad2803a1acd5c45c0c83d34e65cff32d11bb0f744e15a6fefb2f594e`  
		Last Modified: Wed, 05 Aug 2020 00:52:40 GMT  
		Size: 105.1 MB (105111495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fc77ba54e521f28a91f70abb568a9a969bd6d4915d44e3a1e48d31610fedde`  
		Last Modified: Wed, 05 Aug 2020 18:04:15 GMT  
		Size: 2.6 MB (2614631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154095cd463e8d4303cbe6a969ca45487597d6eb231391a2e083de6f99da2335`  
		Last Modified: Wed, 05 Aug 2020 18:04:19 GMT  
		Size: 50.4 MB (50377495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
