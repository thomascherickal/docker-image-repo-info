## `mongo:4-focal`

```console
$ docker pull mongo@sha256:c5d9deed03026bb0dc896bbd7944a39ca8731d320ef7a52b323df215b94545b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4-focal` - linux; amd64

```console
$ docker pull mongo@sha256:3b239fc0230572e422b71be44034c758ca09334b5c7e84228635610051ba169d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.3 MB (171258648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6e8852ad84e91dd9c6d2aec0fb7e9397311c10e7fe146b252aa13fe49901d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:26:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 01 Oct 2021 05:27:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:27:03 GMT
ENV GOSU_VERSION=1.12
# Fri, 01 Oct 2021 05:27:03 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 01 Oct 2021 05:27:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 01 Oct 2021 05:27:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 01 Oct 2021 05:28:08 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 01 Oct 2021 05:28:08 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 01 Oct 2021 05:28:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 01 Oct 2021 05:28:09 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 01 Oct 2021 05:28:09 GMT
ENV MONGO_MAJOR=4.4
# Fri, 01 Oct 2021 05:28:10 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 01 Oct 2021 05:28:10 GMT
ENV MONGO_VERSION=4.4.9
# Fri, 01 Oct 2021 05:28:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 01 Oct 2021 05:28:28 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 01 Oct 2021 05:28:28 GMT
VOLUME [/data/db /data/configdb]
# Fri, 01 Oct 2021 05:28:28 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Fri, 01 Oct 2021 05:28:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 05:28:29 GMT
EXPOSE 27017
# Fri, 01 Oct 2021 05:28:29 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a49f973a13ed259e90f90d516bfd4e86e1294e08ede4b21ddfc91edb575b5c`  
		Last Modified: Fri, 01 Oct 2021 05:29:53 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d4dd6d90045fa1230831362a51b6b81ea0517b3465770ded77c3a427dc997`  
		Last Modified: Fri, 01 Oct 2021 05:29:54 GMT  
		Size: 3.1 MB (3064401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e410f3a61fe9b9491dc6759a94320308ed31e2a7f55773efd31b149b2dcc5f`  
		Last Modified: Fri, 01 Oct 2021 05:29:54 GMT  
		Size: 6.5 MB (6506405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84513ed7bcb687931b1e7054ac30be79aa065bda2aead342ce9fdf4cf16a8d50`  
		Last Modified: Fri, 01 Oct 2021 05:29:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f961faa63743feb86c2cbab05aa7e7442b56e6132f97c519e357d223e0def`  
		Last Modified: Fri, 01 Oct 2021 05:30:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4146772698ca3431c1981b446afd20317df7907dbe13ee78de1f1f1770e8e9b`  
		Last Modified: Fri, 01 Oct 2021 05:30:35 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d67abd2e683847db2655f3723a9d5836981b48f91dcb22c652a35a5fe4e4d29`  
		Last Modified: Fri, 01 Oct 2021 05:30:52 GMT  
		Size: 133.1 MB (133110491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0930c7be04e9e8029b1e211775a4e5d0c8afeb74ccb4f95f7a668da4a3b15ba4`  
		Last Modified: Fri, 01 Oct 2021 05:30:35 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c583d7bc3a628836cdfffd1ba89e89e8de0c336acdd29cdeaa6ddb919262dafa`  
		Last Modified: Fri, 01 Oct 2021 05:30:35 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:5a0c5448a3718d92e15df9e54e8851fb070ffe7173e94322a65673634afce8b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.4 MB (166437009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a4c9642803e0110a82163c5c79ed57e23bb2ac9349162940e8d2ab67de50548`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 15 Oct 2021 23:55:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 15 Oct 2021 23:55:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 Oct 2021 23:55:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 15 Oct 2021 23:55:40 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 15 Oct 2021 23:55:54 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 15 Oct 2021 23:55:55 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 15 Oct 2021 23:56:51 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 15 Oct 2021 23:56:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 15 Oct 2021 23:56:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 15 Oct 2021 23:56:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 15 Oct 2021 23:56:55 GMT
ENV MONGO_MAJOR=4.4
# Fri, 15 Oct 2021 23:56:56 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 15 Oct 2021 23:56:57 GMT
ENV MONGO_VERSION=4.4.10
# Fri, 15 Oct 2021 23:57:14 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 15 Oct 2021 23:57:15 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 15 Oct 2021 23:57:15 GMT
VOLUME [/data/db /data/configdb]
# Fri, 15 Oct 2021 23:57:17 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Fri, 15 Oct 2021 23:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:57:18 GMT
EXPOSE 27017
# Fri, 15 Oct 2021 23:57:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0be693f64925c436bae72e044b8dc5ceb5f19a7569324dd781093b6c517c300`  
		Last Modified: Sat, 16 Oct 2021 00:00:32 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11360d731fd6115880f8f0ccee5f164eeed2a9c5fe43c9fedd0a5e4cabb5d23`  
		Last Modified: Sat, 16 Oct 2021 00:00:33 GMT  
		Size: 2.9 MB (2911863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6264c5e66545e96a0338e8bfce9eb6b3a0fec1b44eb37b491ea75b92a57046ce`  
		Last Modified: Sat, 16 Oct 2021 00:00:33 GMT  
		Size: 6.2 MB (6248468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb851127da015c54694f02dd13e38efc6465c2f4342632a9d2332e26df53a72`  
		Last Modified: Sat, 16 Oct 2021 00:00:32 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6a9dc0b788b8dc086f37b5dfbd36684e2545f5ce01d723d13a6db818abff18`  
		Last Modified: Sat, 16 Oct 2021 00:01:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307dddef536eeb9fd1099bf897ff25b6f59b7ea4864bbf081f34647e9e4665df`  
		Last Modified: Sat, 16 Oct 2021 00:01:15 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d9290c7a2d81ea92f137fa51eb345880c783e764738c1d1f58448e1cd621a`  
		Last Modified: Sat, 16 Oct 2021 00:01:32 GMT  
		Size: 130.1 MB (130095939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35de6c54d83261dc5930d6d9c9f098cf54c5f4acc65a23c5e6e39070b1770f6b`  
		Last Modified: Sat, 16 Oct 2021 00:01:15 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db602a2125590e54e120e94f1f98ff4813e6e4e7e95b2f4e32e2b788871104c2`  
		Last Modified: Sat, 16 Oct 2021 00:01:15 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
