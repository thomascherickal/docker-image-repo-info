<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `zookeeper`

-	[`zookeeper:3.4`](#zookeeper34)
-	[`zookeeper:3.4.14`](#zookeeper3414)
-	[`zookeeper:3.5`](#zookeeper35)
-	[`zookeeper:3.5.6`](#zookeeper356)
-	[`zookeeper:latest`](#zookeeperlatest)

## `zookeeper:3.4`

```console
$ docker pull zookeeper@sha256:eb85924ebf44d852e23cf7916b5f6cbbf28e188302490b007aaa85657f3a5447
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `zookeeper:3.4` - linux; amd64

```console
$ docker pull zookeeper@sha256:31977cefaf50aee4a6d1fe63fcf0ceea408a38a9c1336c2bd634beebdf10bb21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113917020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cf98592b865539351e49195dfd7a4c2d8fc85025719ebd44f3a6b1ad187ffed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["zkServer.sh","start-foreground"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:28:36 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:28:36 GMT
ENV JAVA_VERSION=8u242
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_URL_VERSION=8u242b08
# Sun, 02 Feb 2020 06:29:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sun, 02 Feb 2020 21:51:14 GMT
ENV ZOO_CONF_DIR=/conf ZOO_DATA_DIR=/data ZOO_DATA_LOG_DIR=/datalog ZOO_LOG_DIR=/logs ZOO_TICK_TIME=2000 ZOO_INIT_LIMIT=5 ZOO_SYNC_LIMIT=2 ZOO_AUTOPURGE_PURGEINTERVAL=0 ZOO_AUTOPURGE_SNAPRETAINCOUNT=3 ZOO_MAX_CLIENT_CNXNS=60
# Sun, 02 Feb 2020 21:51:15 GMT
RUN set -eux;     groupadd -r zookeeper --gid=1000;     useradd -r -g zookeeper --uid=1000 zookeeper;     mkdir -p "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR";     chown zookeeper:zookeeper "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR"
# Sun, 02 Feb 2020 21:51:22 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         dirmngr         gosu         gnupg         netcat         wget;     rm -rf /var/lib/apt/lists/*;     gosu nobody true
# Sun, 02 Feb 2020 21:51:22 GMT
ARG GPG_KEY=3F7A1D16FA4217B1DC75E1C9FFE35B7F15DFA1BA
# Sun, 02 Feb 2020 21:51:22 GMT
ARG DISTRO_NAME=zookeeper-3.4.14
# Sun, 02 Feb 2020 21:51:26 GMT
# ARGS: DISTRO_NAME=zookeeper-3.4.14 GPG_KEY=3F7A1D16FA4217B1DC75E1C9FFE35B7F15DFA1BA
RUN set -eux;     ddist() {         local f="$1"; shift;         local distFile="$1"; shift;         local success=;         local distUrl=;         for distUrl in             'https://www.apache.org/dyn/closer.cgi?action=download&filename='             https://www-us.apache.org/dist/             https://www.apache.org/dist/             https://archive.apache.org/dist/         ; do             if wget -q -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then                 success=1;                 break;             fi;         done;         [ -n "$success" ];     };     ddist "$DISTRO_NAME.tar.gz" "zookeeper/$DISTRO_NAME/$DISTRO_NAME.tar.gz";     ddist "$DISTRO_NAME.tar.gz.asc" "zookeeper/$DISTRO_NAME/$DISTRO_NAME.tar.gz.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --keyserver ha.pool.sks-keyservers.net --recv-key "$GPG_KEY" ||     gpg --keyserver pgp.mit.edu --recv-keys "$GPG_KEY" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$GPG_KEY";     gpg --batch --verify "$DISTRO_NAME.tar.gz.asc" "$DISTRO_NAME.tar.gz";     tar -xzf "$DISTRO_NAME.tar.gz";     mv "$DISTRO_NAME/conf/"* "$ZOO_CONF_DIR";     rm -rf "$GNUPGHOME" "$DISTRO_NAME.tar.gz" "$DISTRO_NAME.tar.gz.asc";     chown -R zookeeper:zookeeper "/$DISTRO_NAME"
# Sun, 02 Feb 2020 21:51:26 GMT
WORKDIR /zookeeper-3.4.14
# Sun, 02 Feb 2020 21:51:26 GMT
VOLUME [/data /datalog /logs]
# Sun, 02 Feb 2020 21:51:26 GMT
EXPOSE 2181 2888 3888
# Sun, 02 Feb 2020 21:51:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/zookeeper-3.4.14/bin ZOOCFGDIR=/conf
# Sun, 02 Feb 2020 21:51:27 GMT
COPY file:5f362d86c1b0921aaa8d5421f87e151d62b99d9532beeba5ec2b708b04e7e122 in / 
# Sun, 02 Feb 2020 21:51:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:51:27 GMT
CMD ["zkServer.sh" "start-foreground"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4836bf357bc05fde276db1412eb17d9c5ae12fc0751947bd3cbef5879f5ee955`  
		Last Modified: Sun, 02 Feb 2020 06:37:35 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f042015d97a409ed97493758ab8a8358cd42e3f8b679932768a5d88da51bd38`  
		Last Modified: Sun, 02 Feb 2020 06:38:24 GMT  
		Size: 40.5 MB (40464343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150b72ca97aaabda9b59118b1d68b60582e92076e23197a6a2290735f8ce8972`  
		Last Modified: Sun, 02 Feb 2020 21:51:56 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6bc57509d31a4f0329b141f4ed3607671db616b437524056035ccd638627e9`  
		Last Modified: Sun, 02 Feb 2020 21:51:57 GMT  
		Size: 5.4 MB (5382189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3aed9fd3c5f5e4ec5b9fe23eac5c77b0519f27d836f91358c0652458f4ae29`  
		Last Modified: Sun, 02 Feb 2020 21:52:00 GMT  
		Size: 37.7 MB (37726485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36254ce99ac50d8d846393094b18bb6ac38e7ec0c0da8eda79dac2fccb8da39b`  
		Last Modified: Sun, 02 Feb 2020 21:51:56 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `zookeeper:3.4.14`

```console
$ docker pull zookeeper@sha256:eb85924ebf44d852e23cf7916b5f6cbbf28e188302490b007aaa85657f3a5447
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `zookeeper:3.4.14` - linux; amd64

```console
$ docker pull zookeeper@sha256:31977cefaf50aee4a6d1fe63fcf0ceea408a38a9c1336c2bd634beebdf10bb21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113917020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cf98592b865539351e49195dfd7a4c2d8fc85025719ebd44f3a6b1ad187ffed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["zkServer.sh","start-foreground"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:28:36 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:28:36 GMT
ENV JAVA_VERSION=8u242
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_URL_VERSION=8u242b08
# Sun, 02 Feb 2020 06:29:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sun, 02 Feb 2020 21:51:14 GMT
ENV ZOO_CONF_DIR=/conf ZOO_DATA_DIR=/data ZOO_DATA_LOG_DIR=/datalog ZOO_LOG_DIR=/logs ZOO_TICK_TIME=2000 ZOO_INIT_LIMIT=5 ZOO_SYNC_LIMIT=2 ZOO_AUTOPURGE_PURGEINTERVAL=0 ZOO_AUTOPURGE_SNAPRETAINCOUNT=3 ZOO_MAX_CLIENT_CNXNS=60
# Sun, 02 Feb 2020 21:51:15 GMT
RUN set -eux;     groupadd -r zookeeper --gid=1000;     useradd -r -g zookeeper --uid=1000 zookeeper;     mkdir -p "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR";     chown zookeeper:zookeeper "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR"
# Sun, 02 Feb 2020 21:51:22 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         dirmngr         gosu         gnupg         netcat         wget;     rm -rf /var/lib/apt/lists/*;     gosu nobody true
# Sun, 02 Feb 2020 21:51:22 GMT
ARG GPG_KEY=3F7A1D16FA4217B1DC75E1C9FFE35B7F15DFA1BA
# Sun, 02 Feb 2020 21:51:22 GMT
ARG DISTRO_NAME=zookeeper-3.4.14
# Sun, 02 Feb 2020 21:51:26 GMT
# ARGS: DISTRO_NAME=zookeeper-3.4.14 GPG_KEY=3F7A1D16FA4217B1DC75E1C9FFE35B7F15DFA1BA
RUN set -eux;     ddist() {         local f="$1"; shift;         local distFile="$1"; shift;         local success=;         local distUrl=;         for distUrl in             'https://www.apache.org/dyn/closer.cgi?action=download&filename='             https://www-us.apache.org/dist/             https://www.apache.org/dist/             https://archive.apache.org/dist/         ; do             if wget -q -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then                 success=1;                 break;             fi;         done;         [ -n "$success" ];     };     ddist "$DISTRO_NAME.tar.gz" "zookeeper/$DISTRO_NAME/$DISTRO_NAME.tar.gz";     ddist "$DISTRO_NAME.tar.gz.asc" "zookeeper/$DISTRO_NAME/$DISTRO_NAME.tar.gz.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --keyserver ha.pool.sks-keyservers.net --recv-key "$GPG_KEY" ||     gpg --keyserver pgp.mit.edu --recv-keys "$GPG_KEY" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$GPG_KEY";     gpg --batch --verify "$DISTRO_NAME.tar.gz.asc" "$DISTRO_NAME.tar.gz";     tar -xzf "$DISTRO_NAME.tar.gz";     mv "$DISTRO_NAME/conf/"* "$ZOO_CONF_DIR";     rm -rf "$GNUPGHOME" "$DISTRO_NAME.tar.gz" "$DISTRO_NAME.tar.gz.asc";     chown -R zookeeper:zookeeper "/$DISTRO_NAME"
# Sun, 02 Feb 2020 21:51:26 GMT
WORKDIR /zookeeper-3.4.14
# Sun, 02 Feb 2020 21:51:26 GMT
VOLUME [/data /datalog /logs]
# Sun, 02 Feb 2020 21:51:26 GMT
EXPOSE 2181 2888 3888
# Sun, 02 Feb 2020 21:51:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/zookeeper-3.4.14/bin ZOOCFGDIR=/conf
# Sun, 02 Feb 2020 21:51:27 GMT
COPY file:5f362d86c1b0921aaa8d5421f87e151d62b99d9532beeba5ec2b708b04e7e122 in / 
# Sun, 02 Feb 2020 21:51:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:51:27 GMT
CMD ["zkServer.sh" "start-foreground"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4836bf357bc05fde276db1412eb17d9c5ae12fc0751947bd3cbef5879f5ee955`  
		Last Modified: Sun, 02 Feb 2020 06:37:35 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f042015d97a409ed97493758ab8a8358cd42e3f8b679932768a5d88da51bd38`  
		Last Modified: Sun, 02 Feb 2020 06:38:24 GMT  
		Size: 40.5 MB (40464343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150b72ca97aaabda9b59118b1d68b60582e92076e23197a6a2290735f8ce8972`  
		Last Modified: Sun, 02 Feb 2020 21:51:56 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6bc57509d31a4f0329b141f4ed3607671db616b437524056035ccd638627e9`  
		Last Modified: Sun, 02 Feb 2020 21:51:57 GMT  
		Size: 5.4 MB (5382189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3aed9fd3c5f5e4ec5b9fe23eac5c77b0519f27d836f91358c0652458f4ae29`  
		Last Modified: Sun, 02 Feb 2020 21:52:00 GMT  
		Size: 37.7 MB (37726485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36254ce99ac50d8d846393094b18bb6ac38e7ec0c0da8eda79dac2fccb8da39b`  
		Last Modified: Sun, 02 Feb 2020 21:51:56 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `zookeeper:3.5`

```console
$ docker pull zookeeper@sha256:5b32b799392ee1a605487480e59b134ef71c5fb4fda6ef4b926b6e0081ec9c72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `zookeeper:3.5` - linux; amd64

```console
$ docker pull zookeeper@sha256:5c8f35b7e220c3455fb57cb3c58b55a1c255866bad2a44098afd03d1a02d19aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85327748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e30cac00aca1bb8ebd48bbbe5447226406c7d53fba2f66d57af9ee146524571`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["zkServer.sh","start-foreground"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:28:36 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:28:36 GMT
ENV JAVA_VERSION=8u242
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_URL_VERSION=8u242b08
# Sun, 02 Feb 2020 06:29:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sun, 02 Feb 2020 21:51:32 GMT
ENV ZOO_CONF_DIR=/conf ZOO_DATA_DIR=/data ZOO_DATA_LOG_DIR=/datalog ZOO_LOG_DIR=/logs ZOO_TICK_TIME=2000 ZOO_INIT_LIMIT=5 ZOO_SYNC_LIMIT=2 ZOO_AUTOPURGE_PURGEINTERVAL=0 ZOO_AUTOPURGE_SNAPRETAINCOUNT=3 ZOO_MAX_CLIENT_CNXNS=60 ZOO_STANDALONE_ENABLED=true ZOO_ADMINSERVER_ENABLED=true
# Sun, 02 Feb 2020 21:51:33 GMT
RUN set -eux;     groupadd -r zookeeper --gid=1000;     useradd -r -g zookeeper --uid=1000 zookeeper;     mkdir -p "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR";     chown zookeeper:zookeeper "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR"
# Sun, 02 Feb 2020 21:51:39 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         dirmngr         gosu         gnupg         netcat         wget;     rm -rf /var/lib/apt/lists/*;     gosu nobody true
# Sun, 02 Feb 2020 21:51:39 GMT
ARG GPG_KEY=BBE7232D7991050B54C8EA0ADC08637CA615D22C
# Sun, 02 Feb 2020 21:51:40 GMT
ARG SHORT_DISTRO_NAME=zookeeper-3.5.6
# Sun, 02 Feb 2020 21:51:40 GMT
ARG DISTRO_NAME=apache-zookeeper-3.5.6-bin
# Sun, 02 Feb 2020 21:51:46 GMT
# ARGS: DISTRO_NAME=apache-zookeeper-3.5.6-bin GPG_KEY=BBE7232D7991050B54C8EA0ADC08637CA615D22C SHORT_DISTRO_NAME=zookeeper-3.5.6
RUN set -eux;     ddist() {         local f="$1"; shift;         local distFile="$1"; shift;         local success=;         local distUrl=;         for distUrl in             'https://www.apache.org/dyn/closer.cgi?action=download&filename='             https://www-us.apache.org/dist/             https://www.apache.org/dist/             https://archive.apache.org/dist/         ; do             if wget -q -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then                 success=1;                 break;             fi;         done;         [ -n "$success" ];     };     ddist "$DISTRO_NAME.tar.gz" "zookeeper/$SHORT_DISTRO_NAME/$DISTRO_NAME.tar.gz";     ddist "$DISTRO_NAME.tar.gz.asc" "zookeeper/$SHORT_DISTRO_NAME/$DISTRO_NAME.tar.gz.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --keyserver ha.pool.sks-keyservers.net --recv-key "$GPG_KEY" ||     gpg --keyserver pgp.mit.edu --recv-keys "$GPG_KEY" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$GPG_KEY";     gpg --batch --verify "$DISTRO_NAME.tar.gz.asc" "$DISTRO_NAME.tar.gz";     tar -zxf "$DISTRO_NAME.tar.gz";     mv "$DISTRO_NAME/conf/"* "$ZOO_CONF_DIR";     rm -rf "$GNUPGHOME" "$DISTRO_NAME.tar.gz" "$DISTRO_NAME.tar.gz.asc";     chown -R zookeeper:zookeeper "/$DISTRO_NAME"
# Sun, 02 Feb 2020 21:51:46 GMT
WORKDIR /apache-zookeeper-3.5.6-bin
# Sun, 02 Feb 2020 21:51:46 GMT
VOLUME [/data /datalog /logs]
# Sun, 02 Feb 2020 21:51:46 GMT
EXPOSE 2181 2888 3888 8080
# Sun, 02 Feb 2020 21:51:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/apache-zookeeper-3.5.6-bin/bin ZOOCFGDIR=/conf
# Sun, 02 Feb 2020 21:51:47 GMT
COPY file:5b1c80c9153f745576365153bfff6220ee6e01a20293b15f8cb10a5dafe1fd83 in / 
# Sun, 02 Feb 2020 21:51:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:51:47 GMT
CMD ["zkServer.sh" "start-foreground"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4836bf357bc05fde276db1412eb17d9c5ae12fc0751947bd3cbef5879f5ee955`  
		Last Modified: Sun, 02 Feb 2020 06:37:35 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f042015d97a409ed97493758ab8a8358cd42e3f8b679932768a5d88da51bd38`  
		Last Modified: Sun, 02 Feb 2020 06:38:24 GMT  
		Size: 40.5 MB (40464343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cf0aeabc1ad051167d6c26c579e54e5103300ee3608c1f3361a579c056fb22`  
		Last Modified: Sun, 02 Feb 2020 21:52:04 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9283fb10d6791315aa3461c8e0a44207283522844663c662d59f5ab1dba099a5`  
		Last Modified: Sun, 02 Feb 2020 21:52:05 GMT  
		Size: 5.4 MB (5382219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515c4b0b2ed3077a3bf62ec477b732bc4d3b2e2c57a32f3ed0ea0a646d4e78ca`  
		Last Modified: Sun, 02 Feb 2020 21:52:05 GMT  
		Size: 9.1 MB (9137053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1f94696317884be0682429b7e7e72acfe4c7aca68151307d1f5cd897fe4dec`  
		Last Modified: Sun, 02 Feb 2020 21:52:04 GMT  
		Size: 748.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `zookeeper:3.5.6`

```console
$ docker pull zookeeper@sha256:5b32b799392ee1a605487480e59b134ef71c5fb4fda6ef4b926b6e0081ec9c72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `zookeeper:3.5.6` - linux; amd64

```console
$ docker pull zookeeper@sha256:5c8f35b7e220c3455fb57cb3c58b55a1c255866bad2a44098afd03d1a02d19aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85327748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e30cac00aca1bb8ebd48bbbe5447226406c7d53fba2f66d57af9ee146524571`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["zkServer.sh","start-foreground"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:28:36 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:28:36 GMT
ENV JAVA_VERSION=8u242
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_URL_VERSION=8u242b08
# Sun, 02 Feb 2020 06:29:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sun, 02 Feb 2020 21:51:32 GMT
ENV ZOO_CONF_DIR=/conf ZOO_DATA_DIR=/data ZOO_DATA_LOG_DIR=/datalog ZOO_LOG_DIR=/logs ZOO_TICK_TIME=2000 ZOO_INIT_LIMIT=5 ZOO_SYNC_LIMIT=2 ZOO_AUTOPURGE_PURGEINTERVAL=0 ZOO_AUTOPURGE_SNAPRETAINCOUNT=3 ZOO_MAX_CLIENT_CNXNS=60 ZOO_STANDALONE_ENABLED=true ZOO_ADMINSERVER_ENABLED=true
# Sun, 02 Feb 2020 21:51:33 GMT
RUN set -eux;     groupadd -r zookeeper --gid=1000;     useradd -r -g zookeeper --uid=1000 zookeeper;     mkdir -p "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR";     chown zookeeper:zookeeper "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR"
# Sun, 02 Feb 2020 21:51:39 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         dirmngr         gosu         gnupg         netcat         wget;     rm -rf /var/lib/apt/lists/*;     gosu nobody true
# Sun, 02 Feb 2020 21:51:39 GMT
ARG GPG_KEY=BBE7232D7991050B54C8EA0ADC08637CA615D22C
# Sun, 02 Feb 2020 21:51:40 GMT
ARG SHORT_DISTRO_NAME=zookeeper-3.5.6
# Sun, 02 Feb 2020 21:51:40 GMT
ARG DISTRO_NAME=apache-zookeeper-3.5.6-bin
# Sun, 02 Feb 2020 21:51:46 GMT
# ARGS: DISTRO_NAME=apache-zookeeper-3.5.6-bin GPG_KEY=BBE7232D7991050B54C8EA0ADC08637CA615D22C SHORT_DISTRO_NAME=zookeeper-3.5.6
RUN set -eux;     ddist() {         local f="$1"; shift;         local distFile="$1"; shift;         local success=;         local distUrl=;         for distUrl in             'https://www.apache.org/dyn/closer.cgi?action=download&filename='             https://www-us.apache.org/dist/             https://www.apache.org/dist/             https://archive.apache.org/dist/         ; do             if wget -q -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then                 success=1;                 break;             fi;         done;         [ -n "$success" ];     };     ddist "$DISTRO_NAME.tar.gz" "zookeeper/$SHORT_DISTRO_NAME/$DISTRO_NAME.tar.gz";     ddist "$DISTRO_NAME.tar.gz.asc" "zookeeper/$SHORT_DISTRO_NAME/$DISTRO_NAME.tar.gz.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --keyserver ha.pool.sks-keyservers.net --recv-key "$GPG_KEY" ||     gpg --keyserver pgp.mit.edu --recv-keys "$GPG_KEY" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$GPG_KEY";     gpg --batch --verify "$DISTRO_NAME.tar.gz.asc" "$DISTRO_NAME.tar.gz";     tar -zxf "$DISTRO_NAME.tar.gz";     mv "$DISTRO_NAME/conf/"* "$ZOO_CONF_DIR";     rm -rf "$GNUPGHOME" "$DISTRO_NAME.tar.gz" "$DISTRO_NAME.tar.gz.asc";     chown -R zookeeper:zookeeper "/$DISTRO_NAME"
# Sun, 02 Feb 2020 21:51:46 GMT
WORKDIR /apache-zookeeper-3.5.6-bin
# Sun, 02 Feb 2020 21:51:46 GMT
VOLUME [/data /datalog /logs]
# Sun, 02 Feb 2020 21:51:46 GMT
EXPOSE 2181 2888 3888 8080
# Sun, 02 Feb 2020 21:51:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/apache-zookeeper-3.5.6-bin/bin ZOOCFGDIR=/conf
# Sun, 02 Feb 2020 21:51:47 GMT
COPY file:5b1c80c9153f745576365153bfff6220ee6e01a20293b15f8cb10a5dafe1fd83 in / 
# Sun, 02 Feb 2020 21:51:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:51:47 GMT
CMD ["zkServer.sh" "start-foreground"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4836bf357bc05fde276db1412eb17d9c5ae12fc0751947bd3cbef5879f5ee955`  
		Last Modified: Sun, 02 Feb 2020 06:37:35 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f042015d97a409ed97493758ab8a8358cd42e3f8b679932768a5d88da51bd38`  
		Last Modified: Sun, 02 Feb 2020 06:38:24 GMT  
		Size: 40.5 MB (40464343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cf0aeabc1ad051167d6c26c579e54e5103300ee3608c1f3361a579c056fb22`  
		Last Modified: Sun, 02 Feb 2020 21:52:04 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9283fb10d6791315aa3461c8e0a44207283522844663c662d59f5ab1dba099a5`  
		Last Modified: Sun, 02 Feb 2020 21:52:05 GMT  
		Size: 5.4 MB (5382219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515c4b0b2ed3077a3bf62ec477b732bc4d3b2e2c57a32f3ed0ea0a646d4e78ca`  
		Last Modified: Sun, 02 Feb 2020 21:52:05 GMT  
		Size: 9.1 MB (9137053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1f94696317884be0682429b7e7e72acfe4c7aca68151307d1f5cd897fe4dec`  
		Last Modified: Sun, 02 Feb 2020 21:52:04 GMT  
		Size: 748.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `zookeeper:latest`

```console
$ docker pull zookeeper@sha256:5b32b799392ee1a605487480e59b134ef71c5fb4fda6ef4b926b6e0081ec9c72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `zookeeper:latest` - linux; amd64

```console
$ docker pull zookeeper@sha256:5c8f35b7e220c3455fb57cb3c58b55a1c255866bad2a44098afd03d1a02d19aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85327748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e30cac00aca1bb8ebd48bbbe5447226406c7d53fba2f66d57af9ee146524571`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["zkServer.sh","start-foreground"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sun, 02 Feb 2020 06:28:34 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:28:36 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:28:36 GMT
ENV JAVA_VERSION=8u242
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Sun, 02 Feb 2020 06:29:19 GMT
ENV JAVA_URL_VERSION=8u242b08
# Sun, 02 Feb 2020 06:29:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sun, 02 Feb 2020 21:51:32 GMT
ENV ZOO_CONF_DIR=/conf ZOO_DATA_DIR=/data ZOO_DATA_LOG_DIR=/datalog ZOO_LOG_DIR=/logs ZOO_TICK_TIME=2000 ZOO_INIT_LIMIT=5 ZOO_SYNC_LIMIT=2 ZOO_AUTOPURGE_PURGEINTERVAL=0 ZOO_AUTOPURGE_SNAPRETAINCOUNT=3 ZOO_MAX_CLIENT_CNXNS=60 ZOO_STANDALONE_ENABLED=true ZOO_ADMINSERVER_ENABLED=true
# Sun, 02 Feb 2020 21:51:33 GMT
RUN set -eux;     groupadd -r zookeeper --gid=1000;     useradd -r -g zookeeper --uid=1000 zookeeper;     mkdir -p "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR";     chown zookeeper:zookeeper "$ZOO_DATA_LOG_DIR" "$ZOO_DATA_DIR" "$ZOO_CONF_DIR" "$ZOO_LOG_DIR"
# Sun, 02 Feb 2020 21:51:39 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         dirmngr         gosu         gnupg         netcat         wget;     rm -rf /var/lib/apt/lists/*;     gosu nobody true
# Sun, 02 Feb 2020 21:51:39 GMT
ARG GPG_KEY=BBE7232D7991050B54C8EA0ADC08637CA615D22C
# Sun, 02 Feb 2020 21:51:40 GMT
ARG SHORT_DISTRO_NAME=zookeeper-3.5.6
# Sun, 02 Feb 2020 21:51:40 GMT
ARG DISTRO_NAME=apache-zookeeper-3.5.6-bin
# Sun, 02 Feb 2020 21:51:46 GMT
# ARGS: DISTRO_NAME=apache-zookeeper-3.5.6-bin GPG_KEY=BBE7232D7991050B54C8EA0ADC08637CA615D22C SHORT_DISTRO_NAME=zookeeper-3.5.6
RUN set -eux;     ddist() {         local f="$1"; shift;         local distFile="$1"; shift;         local success=;         local distUrl=;         for distUrl in             'https://www.apache.org/dyn/closer.cgi?action=download&filename='             https://www-us.apache.org/dist/             https://www.apache.org/dist/             https://archive.apache.org/dist/         ; do             if wget -q -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then                 success=1;                 break;             fi;         done;         [ -n "$success" ];     };     ddist "$DISTRO_NAME.tar.gz" "zookeeper/$SHORT_DISTRO_NAME/$DISTRO_NAME.tar.gz";     ddist "$DISTRO_NAME.tar.gz.asc" "zookeeper/$SHORT_DISTRO_NAME/$DISTRO_NAME.tar.gz.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --keyserver ha.pool.sks-keyservers.net --recv-key "$GPG_KEY" ||     gpg --keyserver pgp.mit.edu --recv-keys "$GPG_KEY" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$GPG_KEY";     gpg --batch --verify "$DISTRO_NAME.tar.gz.asc" "$DISTRO_NAME.tar.gz";     tar -zxf "$DISTRO_NAME.tar.gz";     mv "$DISTRO_NAME/conf/"* "$ZOO_CONF_DIR";     rm -rf "$GNUPGHOME" "$DISTRO_NAME.tar.gz" "$DISTRO_NAME.tar.gz.asc";     chown -R zookeeper:zookeeper "/$DISTRO_NAME"
# Sun, 02 Feb 2020 21:51:46 GMT
WORKDIR /apache-zookeeper-3.5.6-bin
# Sun, 02 Feb 2020 21:51:46 GMT
VOLUME [/data /datalog /logs]
# Sun, 02 Feb 2020 21:51:46 GMT
EXPOSE 2181 2888 3888 8080
# Sun, 02 Feb 2020 21:51:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/apache-zookeeper-3.5.6-bin/bin ZOOCFGDIR=/conf
# Sun, 02 Feb 2020 21:51:47 GMT
COPY file:5b1c80c9153f745576365153bfff6220ee6e01a20293b15f8cb10a5dafe1fd83 in / 
# Sun, 02 Feb 2020 21:51:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:51:47 GMT
CMD ["zkServer.sh" "start-foreground"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4836bf357bc05fde276db1412eb17d9c5ae12fc0751947bd3cbef5879f5ee955`  
		Last Modified: Sun, 02 Feb 2020 06:37:35 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f042015d97a409ed97493758ab8a8358cd42e3f8b679932768a5d88da51bd38`  
		Last Modified: Sun, 02 Feb 2020 06:38:24 GMT  
		Size: 40.5 MB (40464343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cf0aeabc1ad051167d6c26c579e54e5103300ee3608c1f3361a579c056fb22`  
		Last Modified: Sun, 02 Feb 2020 21:52:04 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9283fb10d6791315aa3461c8e0a44207283522844663c662d59f5ab1dba099a5`  
		Last Modified: Sun, 02 Feb 2020 21:52:05 GMT  
		Size: 5.4 MB (5382219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515c4b0b2ed3077a3bf62ec477b732bc4d3b2e2c57a32f3ed0ea0a646d4e78ca`  
		Last Modified: Sun, 02 Feb 2020 21:52:05 GMT  
		Size: 9.1 MB (9137053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1f94696317884be0682429b7e7e72acfe4c7aca68151307d1f5cd897fe4dec`  
		Last Modified: Sun, 02 Feb 2020 21:52:04 GMT  
		Size: 748.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
