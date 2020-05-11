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
-	[`orientdb:3.0.31`](#orientdb3031)
-	[`orientdb:3.0.31-tp3`](#orientdb3031-tp3)
-	[`orientdb:3.0-tp3`](#orientdb30-tp3)
-	[`orientdb:latest`](#orientdblatest)

## `orientdb:2.0`

```console
$ docker pull orientdb@sha256:01de35ee0f83cf87e635b20e7fa663986775a895b09d79fcc43732edb2097a64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.0` - linux; amd64

```console
$ docker pull orientdb@sha256:3cb7cbf93e0166f2520750f64b1f0bc500bc73bc451b84234efd336e88e1a3b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.3 MB (276331519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399bfcb5879cddbef508aa8dec3545b1212925e29f4b6b78dc174bef289acc54`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:17 GMT
ADD file:f086177965196842af3c15f50a7f6ad7912aaa7bf73a60b1d00e3129265eec9a in / 
# Thu, 23 Apr 2020 00:20:17 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:50:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 00:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:01:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:01:53 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:05 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:05 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:06 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:06 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:18:49 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:18:49 GMT
ENV ORIENTDB_VERSION=2.0.18
# Thu, 23 Apr 2020 23:18:50 GMT
ENV ORIENTDB_DOWNLOAD_MD5=9e7b7e7b6d95795b188adb4e5898a1b8
# Thu, 23 Apr 2020 23:18:50 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=f562794536bbf8ae2145f96153e58b1e5d9211b3
# Thu, 23 Apr 2020 23:18:54 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:18:54 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:18:55 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:18:55 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:18:55 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:18:55 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:18:56 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:90fe46dd819953eb995f9cc9c326130abe9dd0b3993a998e12c01d0218a0b831`  
		Last Modified: Thu, 23 Apr 2020 00:24:56 GMT  
		Size: 50.4 MB (50382927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a4f197768941ef308d981a94f6d06fb77b9f2ba89dc04d2daf8292ee297315`  
		Last Modified: Thu, 23 Apr 2020 01:02:49 GMT  
		Size: 7.8 MB (7812206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc37f14aded2d49bfac62dfa404755c9f1cadfee2b35933e4906f0054782888`  
		Last Modified: Thu, 23 Apr 2020 01:02:49 GMT  
		Size: 10.0 MB (9996197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e27dc593d49a6d728dfe36976cb1469e076fbf3611e501fd030308cd212a80`  
		Last Modified: Thu, 23 Apr 2020 01:03:03 GMT  
		Size: 51.8 MB (51826941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a01fbfad7fc489eface0e3ea2ca5e8c84746c8300dd06bc5634605666fbf99`  
		Last Modified: Thu, 23 Apr 2020 04:10:32 GMT  
		Size: 5.3 MB (5284595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1478df40586973c72ae11ad4b0733defb36612ac5a39755ac96dee70d564af9a`  
		Last Modified: Thu, 23 Apr 2020 04:12:27 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f0dd11682ba1e8f6f0f9543ad7acbb6b130e91c223eee07b8d5a1b16455963`  
		Last Modified: Thu, 23 Apr 2020 04:12:43 GMT  
		Size: 104.4 MB (104441883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa0cdaedf0927a5c473d1cc0bcc555728014b0588695b4500d55c4190d091b1`  
		Last Modified: Thu, 23 Apr 2020 23:19:41 GMT  
		Size: 46.6 MB (46586558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.0.18`

```console
$ docker pull orientdb@sha256:01de35ee0f83cf87e635b20e7fa663986775a895b09d79fcc43732edb2097a64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.0.18` - linux; amd64

```console
$ docker pull orientdb@sha256:3cb7cbf93e0166f2520750f64b1f0bc500bc73bc451b84234efd336e88e1a3b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.3 MB (276331519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399bfcb5879cddbef508aa8dec3545b1212925e29f4b6b78dc174bef289acc54`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:17 GMT
ADD file:f086177965196842af3c15f50a7f6ad7912aaa7bf73a60b1d00e3129265eec9a in / 
# Thu, 23 Apr 2020 00:20:17 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:50:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:50:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 00:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:01:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:01:53 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:05 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:05 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:06 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:06 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:18:49 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:18:49 GMT
ENV ORIENTDB_VERSION=2.0.18
# Thu, 23 Apr 2020 23:18:50 GMT
ENV ORIENTDB_DOWNLOAD_MD5=9e7b7e7b6d95795b188adb4e5898a1b8
# Thu, 23 Apr 2020 23:18:50 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=f562794536bbf8ae2145f96153e58b1e5d9211b3
# Thu, 23 Apr 2020 23:18:54 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:18:54 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:18:55 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:18:55 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:18:55 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:18:55 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:18:56 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:90fe46dd819953eb995f9cc9c326130abe9dd0b3993a998e12c01d0218a0b831`  
		Last Modified: Thu, 23 Apr 2020 00:24:56 GMT  
		Size: 50.4 MB (50382927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a4f197768941ef308d981a94f6d06fb77b9f2ba89dc04d2daf8292ee297315`  
		Last Modified: Thu, 23 Apr 2020 01:02:49 GMT  
		Size: 7.8 MB (7812206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc37f14aded2d49bfac62dfa404755c9f1cadfee2b35933e4906f0054782888`  
		Last Modified: Thu, 23 Apr 2020 01:02:49 GMT  
		Size: 10.0 MB (9996197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e27dc593d49a6d728dfe36976cb1469e076fbf3611e501fd030308cd212a80`  
		Last Modified: Thu, 23 Apr 2020 01:03:03 GMT  
		Size: 51.8 MB (51826941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a01fbfad7fc489eface0e3ea2ca5e8c84746c8300dd06bc5634605666fbf99`  
		Last Modified: Thu, 23 Apr 2020 04:10:32 GMT  
		Size: 5.3 MB (5284595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1478df40586973c72ae11ad4b0733defb36612ac5a39755ac96dee70d564af9a`  
		Last Modified: Thu, 23 Apr 2020 04:12:27 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f0dd11682ba1e8f6f0f9543ad7acbb6b130e91c223eee07b8d5a1b16455963`  
		Last Modified: Thu, 23 Apr 2020 04:12:43 GMT  
		Size: 104.4 MB (104441883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa0cdaedf0927a5c473d1cc0bcc555728014b0588695b4500d55c4190d091b1`  
		Last Modified: Thu, 23 Apr 2020 23:19:41 GMT  
		Size: 46.6 MB (46586558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.1`

```console
$ docker pull orientdb@sha256:1a86f9c90d70f5313e519b76a219a7ab6d0b429eff247b28a6cdbd1f2a95d79d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.1` - linux; amd64

```console
$ docker pull orientdb@sha256:b4036c35ca821b346516d24f6c145f6a0376a2d8e57a5d6e83d109de34a46c8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168768231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8911e55f69bc97b9fcea61203003d7f7fbacf7f2c392623e97751b1901ac6327`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:59:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:27 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:17:31 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:18:28 GMT
ENV ORIENTDB_VERSION=2.1.25
# Thu, 23 Apr 2020 23:18:28 GMT
ENV ORIENTDB_DOWNLOAD_MD5=054da3fb7c56e7822b2af116966576ce
# Thu, 23 Apr 2020 23:18:28 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=b7b08242b40117ac8eb9a201f8704bde839dfcb8
# Thu, 23 Apr 2020 23:18:37 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 23:18:43 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:18:44 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:18:44 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:18:44 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:18:44 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:18:44 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:18:45 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dd01647a92dedec9093f4872d18b5a91e98a48731a7c9bc733d288be336017`  
		Last Modified: Thu, 23 Apr 2020 04:07:47 GMT  
		Size: 3.2 MB (3249064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb931af9b241b70d07321c65d1cb8a1416d548e86ca8e6933e2734adf039d68e`  
		Last Modified: Thu, 23 Apr 2020 04:12:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8cbae8041edd4d8c351fce0041a1a5e42ff391f481d3686ae1cf98fb0418b`  
		Last Modified: Thu, 23 Apr 2020 04:13:00 GMT  
		Size: 104.7 MB (104718134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d9eb99701e13f13d72feb722fb97737d95f69970105984ac534c6f085e3d89`  
		Last Modified: Thu, 23 Apr 2020 23:19:32 GMT  
		Size: 2.6 MB (2614608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdd2693defe37616a268a089a8a02d489f4f6db819d7181d3b23d8e40559dbe`  
		Last Modified: Thu, 23 Apr 2020 23:19:34 GMT  
		Size: 31.1 MB (31087960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.1.25`

```console
$ docker pull orientdb@sha256:1a86f9c90d70f5313e519b76a219a7ab6d0b429eff247b28a6cdbd1f2a95d79d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.1.25` - linux; amd64

```console
$ docker pull orientdb@sha256:b4036c35ca821b346516d24f6c145f6a0376a2d8e57a5d6e83d109de34a46c8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168768231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8911e55f69bc97b9fcea61203003d7f7fbacf7f2c392623e97751b1901ac6327`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:59:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:27 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:17:31 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:18:28 GMT
ENV ORIENTDB_VERSION=2.1.25
# Thu, 23 Apr 2020 23:18:28 GMT
ENV ORIENTDB_DOWNLOAD_MD5=054da3fb7c56e7822b2af116966576ce
# Thu, 23 Apr 2020 23:18:28 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=b7b08242b40117ac8eb9a201f8704bde839dfcb8
# Thu, 23 Apr 2020 23:18:37 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 23:18:43 GMT
RUN mkdir /orientdb &&   wget  "https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/$ORIENTDB_VERSION/orientdb-community-$ORIENTDB_VERSION.tar.gz"   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1  && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:18:44 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:18:44 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:18:44 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:18:44 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:18:44 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:18:45 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dd01647a92dedec9093f4872d18b5a91e98a48731a7c9bc733d288be336017`  
		Last Modified: Thu, 23 Apr 2020 04:07:47 GMT  
		Size: 3.2 MB (3249064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb931af9b241b70d07321c65d1cb8a1416d548e86ca8e6933e2734adf039d68e`  
		Last Modified: Thu, 23 Apr 2020 04:12:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8cbae8041edd4d8c351fce0041a1a5e42ff391f481d3686ae1cf98fb0418b`  
		Last Modified: Thu, 23 Apr 2020 04:13:00 GMT  
		Size: 104.7 MB (104718134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d9eb99701e13f13d72feb722fb97737d95f69970105984ac534c6f085e3d89`  
		Last Modified: Thu, 23 Apr 2020 23:19:32 GMT  
		Size: 2.6 MB (2614608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdd2693defe37616a268a089a8a02d489f4f6db819d7181d3b23d8e40559dbe`  
		Last Modified: Thu, 23 Apr 2020 23:19:34 GMT  
		Size: 31.1 MB (31087960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2`

```console
$ docker pull orientdb@sha256:3a94e465ef99a7617a7f8dfba42c7eec75710617f1ab2bcec5e610f81eae88a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.2` - linux; amd64

```console
$ docker pull orientdb@sha256:fcc03b71b0fa2c0d37b10e5387901c1cd84cab8cafd2bdd193739dee0e58bcc0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.2 MB (184154158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db749ab14e2f67d332855aab3a8487150b1cbd71fd5316677bdfd57e52a64ca`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:59:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:27 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:17:31 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:17:31 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Thu, 23 Apr 2020 23:18:06 GMT
ENV ORIENTDB_VERSION=2.2.37
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Thu, 23 Apr 2020 23:18:13 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 23:18:17 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:18:17 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:18:17 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:18:18 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:18:18 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:18:18 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:18:18 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dd01647a92dedec9093f4872d18b5a91e98a48731a7c9bc733d288be336017`  
		Last Modified: Thu, 23 Apr 2020 04:07:47 GMT  
		Size: 3.2 MB (3249064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb931af9b241b70d07321c65d1cb8a1416d548e86ca8e6933e2734adf039d68e`  
		Last Modified: Thu, 23 Apr 2020 04:12:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8cbae8041edd4d8c351fce0041a1a5e42ff391f481d3686ae1cf98fb0418b`  
		Last Modified: Thu, 23 Apr 2020 04:13:00 GMT  
		Size: 104.7 MB (104718134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4fee4ea47c1f195bf37728511953fd293f09dbff95921da24d9596bd5db34d`  
		Last Modified: Thu, 23 Apr 2020 23:19:22 GMT  
		Size: 2.6 MB (2614577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011c3dd18174facaae116e243648dd87cbcebe20fefbdbb86772abc4f1815e02`  
		Last Modified: Thu, 23 Apr 2020 23:19:25 GMT  
		Size: 46.5 MB (46473918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2.37`

```console
$ docker pull orientdb@sha256:3a94e465ef99a7617a7f8dfba42c7eec75710617f1ab2bcec5e610f81eae88a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.2.37` - linux; amd64

```console
$ docker pull orientdb@sha256:fcc03b71b0fa2c0d37b10e5387901c1cd84cab8cafd2bdd193739dee0e58bcc0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.2 MB (184154158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db749ab14e2f67d332855aab3a8487150b1cbd71fd5316677bdfd57e52a64ca`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:59:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:27 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:17:31 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:17:31 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Thu, 23 Apr 2020 23:18:06 GMT
ENV ORIENTDB_VERSION=2.2.37
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Thu, 23 Apr 2020 23:18:13 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 23:18:17 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:18:17 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:18:17 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:18:18 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:18:18 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:18:18 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:18:18 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dd01647a92dedec9093f4872d18b5a91e98a48731a7c9bc733d288be336017`  
		Last Modified: Thu, 23 Apr 2020 04:07:47 GMT  
		Size: 3.2 MB (3249064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb931af9b241b70d07321c65d1cb8a1416d548e86ca8e6933e2734adf039d68e`  
		Last Modified: Thu, 23 Apr 2020 04:12:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8cbae8041edd4d8c351fce0041a1a5e42ff391f481d3686ae1cf98fb0418b`  
		Last Modified: Thu, 23 Apr 2020 04:13:00 GMT  
		Size: 104.7 MB (104718134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4fee4ea47c1f195bf37728511953fd293f09dbff95921da24d9596bd5db34d`  
		Last Modified: Thu, 23 Apr 2020 23:19:22 GMT  
		Size: 2.6 MB (2614577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011c3dd18174facaae116e243648dd87cbcebe20fefbdbb86772abc4f1815e02`  
		Last Modified: Thu, 23 Apr 2020 23:19:25 GMT  
		Size: 46.5 MB (46473918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:2.2.37-spatial`

```console
$ docker pull orientdb@sha256:3cabffbf0395cd08c9d597207efd6dcf9fb4a5249bb08040cb8a63d6855d3ad5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:2.2.37-spatial` - linux; amd64

```console
$ docker pull orientdb@sha256:2ac1e7ad538eb9ef434fcd4caec85e2e90c6ff64432ed28d95c6f14a120e8064
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.4 MB (185356740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d390710c85358ffc2b00ddc573071f6d12d7b61b24559a4e8d838839dbbcd39b`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:59:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:27 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:17:31 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:17:31 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Thu, 23 Apr 2020 23:18:06 GMT
ENV ORIENTDB_VERSION=2.2.37
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_MD5=cb80556ef3b0260d0ee5de88ea73fb9d
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=469c402dde029f265fe905de2c08b43960e81f07
# Thu, 23 Apr 2020 23:18:07 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/2.2.37/orientdb-community-2.2.37.tar.gz
# Thu, 23 Apr 2020 23:18:13 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 23:18:17 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:18:17 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:18:17 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:18:18 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:18:18 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:18:18 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:18:18 GMT
CMD ["server.sh"]
# Thu, 23 Apr 2020 23:18:23 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_MD5=9f64ab5e959f5d9ad9ea5195d6d621d2
# Thu, 23 Apr 2020 23:18:23 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_SHA1=1748c9779ea7a8cb8fc068fcabf960e1778e8a19
# Thu, 23 Apr 2020 23:18:23 GMT
ENV ORIENTDB_DOWNLOAD_SPATIAL_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-spatial/2.2.37/orientdb-spatial-2.2.37-dist.jar
# Thu, 23 Apr 2020 23:18:24 GMT
RUN wget $ORIENTDB_DOWNLOAD_SPATIAL_URL     && echo "$ORIENTDB_DOWNLOAD_SPATIAL_MD5 *orientdb-spatial-$ORIENTDB_VERSION-dist.jar" | md5sum -c -     && echo "$ORIENTDB_DOWNLOAD_SPATIAL_SHA1 *orientdb-spatial-$ORIENTDB_VERSION-dist.jar" | sha1sum -c -     && mv orientdb-spatial-*-dist.jar /orientdb/lib/
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dd01647a92dedec9093f4872d18b5a91e98a48731a7c9bc733d288be336017`  
		Last Modified: Thu, 23 Apr 2020 04:07:47 GMT  
		Size: 3.2 MB (3249064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb931af9b241b70d07321c65d1cb8a1416d548e86ca8e6933e2734adf039d68e`  
		Last Modified: Thu, 23 Apr 2020 04:12:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8cbae8041edd4d8c351fce0041a1a5e42ff391f481d3686ae1cf98fb0418b`  
		Last Modified: Thu, 23 Apr 2020 04:13:00 GMT  
		Size: 104.7 MB (104718134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4fee4ea47c1f195bf37728511953fd293f09dbff95921da24d9596bd5db34d`  
		Last Modified: Thu, 23 Apr 2020 23:19:22 GMT  
		Size: 2.6 MB (2614577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011c3dd18174facaae116e243648dd87cbcebe20fefbdbb86772abc4f1815e02`  
		Last Modified: Thu, 23 Apr 2020 23:19:25 GMT  
		Size: 46.5 MB (46473918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce971a48cdf3d1a075da5c77962897889e7387ac6f983ebbd423f1d244560e74`  
		Last Modified: Thu, 23 Apr 2020 23:19:29 GMT  
		Size: 1.2 MB (1202582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0`

```console
$ docker pull orientdb@sha256:37a43ccc3c25440db2434d58b27c7ac64e531172767e2a078b35fbc6ec818ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.0` - linux; amd64

```console
$ docker pull orientdb@sha256:d193008c8fecfcafd2327b0acb9a7d8898d7386d1b0746c225ebc85dff66a9d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.7 MB (174671888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4300cf348240f14b1818f26138db6ff21e42ec9423ebc42e23b28db128c7fa2`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:59:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:27 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:17:31 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:17:31 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Thu, 23 Apr 2020 23:17:32 GMT
ENV ORIENTDB_VERSION=3.0.30
# Thu, 23 Apr 2020 23:17:32 GMT
ENV ORIENTDB_DOWNLOAD_MD5=6929cf30ba4485ddd6dd6b6f924d10fe
# Thu, 23 Apr 2020 23:17:33 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=cd864c8ccc5bb06c2a8516565b6f10e78ce99c49
# Thu, 23 Apr 2020 23:17:33 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.0.30/orientdb-community-3.0.30.tar.gz
# Thu, 23 Apr 2020 23:17:39 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 23:17:43 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:17:43 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:17:43 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:17:43 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:17:44 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:17:44 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:17:44 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dd01647a92dedec9093f4872d18b5a91e98a48731a7c9bc733d288be336017`  
		Last Modified: Thu, 23 Apr 2020 04:07:47 GMT  
		Size: 3.2 MB (3249064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb931af9b241b70d07321c65d1cb8a1416d548e86ca8e6933e2734adf039d68e`  
		Last Modified: Thu, 23 Apr 2020 04:12:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8cbae8041edd4d8c351fce0041a1a5e42ff391f481d3686ae1cf98fb0418b`  
		Last Modified: Thu, 23 Apr 2020 04:13:00 GMT  
		Size: 104.7 MB (104718134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f6b0d65dec69f0549b1a79192f44eeb84e9ad67ee1765c241236feb0e67d0`  
		Last Modified: Thu, 23 Apr 2020 23:19:06 GMT  
		Size: 2.6 MB (2614555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd1bbc60fd1cea7aa5e5c803a1fb5c3e21498ccaf70127be00c607238e28852`  
		Last Modified: Thu, 23 Apr 2020 23:19:09 GMT  
		Size: 37.0 MB (36991670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:3.0.31`

**does not exist** (yet?)

## `orientdb:3.0.31-tp3`

**does not exist** (yet?)

## `orientdb:3.0-tp3`

```console
$ docker pull orientdb@sha256:2f7b36a9f94d071ba4ed73cd7e2f44b953f00446649e85a69464da7a03ddd13b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:3.0-tp3` - linux; amd64

```console
$ docker pull orientdb@sha256:46490d847021f76ffd86f469163617970237450b43a9f2b785a53280defbcfbe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.7 MB (201691611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54454a07caffa3357d389793f56361ffe91f97d955e5c43c664595e4c4df4312`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:59:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:27 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:17:31 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:17:31 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Thu, 23 Apr 2020 23:17:32 GMT
ENV ORIENTDB_VERSION=3.0.30
# Thu, 23 Apr 2020 23:17:48 GMT
ENV ORIENTDB_DOWNLOAD_MD5=092a18540d6939b2208628b00d2ceb4f
# Thu, 23 Apr 2020 23:17:48 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=e1816d36f161d7a57f4e792a9fa0d15cedea22bd
# Thu, 23 Apr 2020 23:17:48 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-tp3/3.0.30/orientdb-tp3-3.0.30.tar.gz
# Thu, 23 Apr 2020 23:17:54 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 23:18:00 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-tp3-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-tp3-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-tp3-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:18:00 GMT
ADD file:5bcd10827429355383b443914a6e6c163692cb388c7594e6e8d3d4625653a011 in /orientdb/config 
# Thu, 23 Apr 2020 23:18:00 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:18:01 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:18:01 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:18:01 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:18:01 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:18:01 GMT
EXPOSE 8182
# Thu, 23 Apr 2020 23:18:02 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dd01647a92dedec9093f4872d18b5a91e98a48731a7c9bc733d288be336017`  
		Last Modified: Thu, 23 Apr 2020 04:07:47 GMT  
		Size: 3.2 MB (3249064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb931af9b241b70d07321c65d1cb8a1416d548e86ca8e6933e2734adf039d68e`  
		Last Modified: Thu, 23 Apr 2020 04:12:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8cbae8041edd4d8c351fce0041a1a5e42ff391f481d3686ae1cf98fb0418b`  
		Last Modified: Thu, 23 Apr 2020 04:13:00 GMT  
		Size: 104.7 MB (104718134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd616a4c16840608661856483d20c206371b74e1ed46a0842ea91d3ecb577a`  
		Last Modified: Thu, 23 Apr 2020 23:19:13 GMT  
		Size: 2.6 MB (2614569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3d414d67027a750e5aa934d78a507b08e30da3a233111a561ddf7853d9bded`  
		Last Modified: Thu, 23 Apr 2020 23:19:18 GMT  
		Size: 64.0 MB (64010002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06288853269649f1d788ed2090a4726ba866158b8de8fd921f09f95aa1809609`  
		Last Modified: Thu, 23 Apr 2020 23:19:13 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `orientdb:latest`

```console
$ docker pull orientdb@sha256:37a43ccc3c25440db2434d58b27c7ac64e531172767e2a078b35fbc6ec818ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `orientdb:latest` - linux; amd64

```console
$ docker pull orientdb@sha256:d193008c8fecfcafd2327b0acb9a7d8898d7386d1b0746c225ebc85dff66a9d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.7 MB (174671888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4300cf348240f14b1818f26138db6ff21e42ec9423ebc42e23b28db128c7fa2`
-	Default Command: `["server.sh"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:59:16 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 23 Apr 2020 04:04:24 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 04:04:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_VERSION=8u252
# Thu, 23 Apr 2020 04:04:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Thu, 23 Apr 2020 04:04:27 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 23 Apr 2020 04:04:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 23 Apr 2020 23:17:31 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Thu, 23 Apr 2020 23:17:31 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Thu, 23 Apr 2020 23:17:32 GMT
ENV ORIENTDB_VERSION=3.0.30
# Thu, 23 Apr 2020 23:17:32 GMT
ENV ORIENTDB_DOWNLOAD_MD5=6929cf30ba4485ddd6dd6b6f924d10fe
# Thu, 23 Apr 2020 23:17:33 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=cd864c8ccc5bb06c2a8516565b6f10e78ce99c49
# Thu, 23 Apr 2020 23:17:33 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.0.30/orientdb-community-3.0.30.tar.gz
# Thu, 23 Apr 2020 23:17:39 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 23:17:43 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Thu, 23 Apr 2020 23:17:43 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 23:17:43 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Thu, 23 Apr 2020 23:17:43 GMT
WORKDIR /orientdb
# Thu, 23 Apr 2020 23:17:44 GMT
EXPOSE 2424
# Thu, 23 Apr 2020 23:17:44 GMT
EXPOSE 2480
# Thu, 23 Apr 2020 23:17:44 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dd01647a92dedec9093f4872d18b5a91e98a48731a7c9bc733d288be336017`  
		Last Modified: Thu, 23 Apr 2020 04:07:47 GMT  
		Size: 3.2 MB (3249064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb931af9b241b70d07321c65d1cb8a1416d548e86ca8e6933e2734adf039d68e`  
		Last Modified: Thu, 23 Apr 2020 04:12:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8cbae8041edd4d8c351fce0041a1a5e42ff391f481d3686ae1cf98fb0418b`  
		Last Modified: Thu, 23 Apr 2020 04:13:00 GMT  
		Size: 104.7 MB (104718134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f6b0d65dec69f0549b1a79192f44eeb84e9ad67ee1765c241236feb0e67d0`  
		Last Modified: Thu, 23 Apr 2020 23:19:06 GMT  
		Size: 2.6 MB (2614555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd1bbc60fd1cea7aa5e5c803a1fb5c3e21498ccaf70127be00c607238e28852`  
		Last Modified: Thu, 23 Apr 2020 23:19:09 GMT  
		Size: 37.0 MB (36991670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
