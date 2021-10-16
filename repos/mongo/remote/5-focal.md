## `mongo:5-focal`

```console
$ docker pull mongo@sha256:125402d054fdcf6c0a1c5974aa33f9a2bcbc976edd8ed2e841de26a3f0bc6cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:5-focal` - linux; amd64

```console
$ docker pull mongo@sha256:af71b1de6636e0819661a0d67ede72947ac4fd8e60d984132ffa9183738a9a82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.5 MB (249537889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a14d3979c54cfd497d225371c3e0403a1481b455cb76187775916348ca9e4e`
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
# Fri, 01 Oct 2021 05:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 01 Oct 2021 05:27:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 01 Oct 2021 05:27:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 01 Oct 2021 05:27:32 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 01 Oct 2021 05:27:32 GMT
ENV MONGO_MAJOR=5.0
# Fri, 01 Oct 2021 05:27:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 01 Oct 2021 05:27:33 GMT
ENV MONGO_VERSION=5.0.3
# Fri, 01 Oct 2021 05:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 01 Oct 2021 05:28:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 01 Oct 2021 05:28:00 GMT
VOLUME [/data/db /data/configdb]
# Fri, 01 Oct 2021 05:28:00 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Fri, 01 Oct 2021 05:28:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 05:28:01 GMT
EXPOSE 27017
# Fri, 01 Oct 2021 05:28:01 GMT
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
	-	`sha256:6c69ef6aac84f33a417053e791c50647b3042ffec8d33c9dfad2ec52c06ba821`  
		Last Modified: Fri, 01 Oct 2021 05:29:51 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc764861fa21f832bce37509cafb48035d10dc8a553d1f2e6910d4c6d8767e1`  
		Last Modified: Fri, 01 Oct 2021 05:29:51 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312d8b37ffda4e2af86a952f762d3dc6dbbf4638ddc151aacadbba9e3299d30`  
		Last Modified: Fri, 01 Oct 2021 05:30:19 GMT  
		Size: 211.4 MB (211389736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f757690572b3fb279e22d555aa3830afd42b562890b8f2386531bd49c64b84`  
		Last Modified: Fri, 01 Oct 2021 05:29:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6327a25cb49090b335dca3053e4cf22e0b7a646e951b198e773c98b11d41a5`  
		Last Modified: Fri, 01 Oct 2021 05:29:51 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:d4c0b9f88ab46421a40dad0cb2265eca17052fbcdce55d10614afffad7c133d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239486492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9962a57a6bd8b67bafd90946a940325af3524ee132efc480c916c3c9edfbadcf`
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
# Fri, 15 Oct 2021 23:56:03 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 15 Oct 2021 23:56:04 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 15 Oct 2021 23:56:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 15 Oct 2021 23:56:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 15 Oct 2021 23:56:07 GMT
ENV MONGO_MAJOR=5.0
# Fri, 15 Oct 2021 23:56:08 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 15 Oct 2021 23:56:09 GMT
ENV MONGO_VERSION=5.0.3
# Fri, 15 Oct 2021 23:56:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 15 Oct 2021 23:56:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 15 Oct 2021 23:56:32 GMT
VOLUME [/data/db /data/configdb]
# Fri, 15 Oct 2021 23:56:34 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Fri, 15 Oct 2021 23:56:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:56:35 GMT
EXPOSE 27017
# Fri, 15 Oct 2021 23:56:36 GMT
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
	-	`sha256:25f195d6c04c7f652fd7138b4f872e19a3a0e4a512a49d26a5d9375f81e4b0e7`  
		Last Modified: Sat, 16 Oct 2021 00:00:30 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321c54b765141bed9e3eefa1f1688e9593cbec37b9198e1429792ad8351fe466`  
		Last Modified: Sat, 16 Oct 2021 00:00:30 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852669abe42dc4a4a27d646927ee600b1071f5ec7956f88aef85ed820ecdb9f8`  
		Last Modified: Sat, 16 Oct 2021 00:00:58 GMT  
		Size: 203.1 MB (203145423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226d993618f109fcda569ba5f2a47d084ba959b2d314c81c7fb8ff3d7ae572d7`  
		Last Modified: Sat, 16 Oct 2021 00:00:30 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46853aeb97392c2b389739eb018d0382b398dc75df2bf4a05909ac193ea8a30a`  
		Last Modified: Sat, 16 Oct 2021 00:00:30 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
