## `mongo:4-focal`

```console
$ docker pull mongo@sha256:c1718a46a7e4b1948cd13241fe40d83e317f50484b86d89d37fedacd8dd25539
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4-focal` - linux; amd64

```console
$ docker pull mongo@sha256:ee65af0fa96396530ba2c48db6c2411d9f66186773a57f3428484f8f0674f8aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171122796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409f644a06fccdb5dddf3be89f7a09542b222f20630f9a0009e66989f16cfe99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:19:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 27 Jul 2021 00:19:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:19:09 GMT
ENV GOSU_VERSION=1.12
# Tue, 27 Jul 2021 00:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 27 Jul 2021 00:19:20 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:19:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:20:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:20:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Tue, 27 Jul 2021 00:20:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Tue, 27 Jul 2021 00:20:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Tue, 27 Jul 2021 00:20:02 GMT
ENV MONGO_MAJOR=4.4
# Tue, 27 Jul 2021 00:20:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 27 Jul 2021 00:20:03 GMT
ENV MONGO_VERSION=4.4.7
# Tue, 27 Jul 2021 00:20:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 27 Jul 2021 00:20:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 27 Jul 2021 00:20:21 GMT
VOLUME [/data/db /data/configdb]
# Wed, 04 Aug 2021 21:29:27 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Wed, 04 Aug 2021 21:29:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 21:29:27 GMT
EXPOSE 27017
# Wed, 04 Aug 2021 21:29:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6335cf672677ce540e0f02f99098fdbb5fe6c11e4322a415119dd06f3be5c0a0`  
		Last Modified: Tue, 27 Jul 2021 00:23:01 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc70ccc8ebe91e13d0460b1b78df150627a7bfc892b2c6cc87112b06dcd2eb6`  
		Last Modified: Tue, 27 Jul 2021 00:22:59 GMT  
		Size: 3.1 MB (3063745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1a3c6bd4175a271cffe4b4ea115ba6b94fa4fff3080aea88bf69c8fd3f281c`  
		Last Modified: Tue, 27 Jul 2021 00:22:59 GMT  
		Size: 6.5 MB (6505864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960f3b9b27d33484b86cc838f3f5c815a0d06833e1af863dedaedc06dfa1b514`  
		Last Modified: Tue, 27 Jul 2021 00:22:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f84a5111fd42c20bba4c0178b859910f43192640ced63de2d296936bc39c233`  
		Last Modified: Tue, 27 Jul 2021 00:23:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d124bca258f0a64720d24ec360945a79ae47a5791952e26610af528e06ae1b98`  
		Last Modified: Tue, 27 Jul 2021 00:23:45 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50586751bc65cf11f122eb9ccedb400c0072d9b0b4a8c35ca92d651b65dc228`  
		Last Modified: Tue, 27 Jul 2021 00:24:02 GMT  
		Size: 133.0 MB (132976811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b72a108f7a87ae33df411c5b67c2abc6bfccadc3fadef2ae0e80a1072e88282`  
		Last Modified: Tue, 27 Jul 2021 00:23:45 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4772e9e25705d11971b4469d5b0ad659a75e2bf7f3596e1357b7499632cd93a`  
		Last Modified: Wed, 04 Aug 2021 21:30:30 GMT  
		Size: 4.7 KB (4696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:0c1bb9339a5f11bde9acb9d51fa851748ae0a4bdcbfd23e87e967753bace389b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.4 MB (166413287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea35bd86c85634fadac25aa0d1ac6dbb0858d9a6dd3485566f4e7768ea22511`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:28:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 26 Jul 2021 23:28:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:28:57 GMT
ENV GOSU_VERSION=1.12
# Mon, 26 Jul 2021 23:28:57 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 26 Jul 2021 23:29:11 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 26 Jul 2021 23:29:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 26 Jul 2021 23:29:51 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 26 Jul 2021 23:29:51 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 26 Jul 2021 23:29:51 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 26 Jul 2021 23:29:51 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 26 Jul 2021 23:29:51 GMT
ENV MONGO_MAJOR=4.4
# Mon, 26 Jul 2021 23:29:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 04 Aug 2021 23:40:14 GMT
ENV MONGO_VERSION=4.4.8
# Wed, 04 Aug 2021 23:40:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 04 Aug 2021 23:40:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 04 Aug 2021 23:40:32 GMT
VOLUME [/data/db /data/configdb]
# Wed, 04 Aug 2021 23:40:32 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Wed, 04 Aug 2021 23:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Aug 2021 23:40:33 GMT
EXPOSE 27017
# Wed, 04 Aug 2021 23:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c078c670449119708548deb73fc4b2367fa17e7aa2ccf7d9635f052a393175d7`  
		Last Modified: Mon, 26 Jul 2021 23:32:50 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d7ca682de71cc0d28d5a25c21dcd26bce98321effac96e7c222cad612f192f`  
		Last Modified: Mon, 26 Jul 2021 23:32:51 GMT  
		Size: 2.9 MB (2913005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1276b06a5f9112b01253aa3f54e3998c37b6a78454d9c53873756a9feb2852d1`  
		Last Modified: Mon, 26 Jul 2021 23:32:52 GMT  
		Size: 6.4 MB (6406013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b013f927ec79564222ec0dc72cf65f4fe208c8cb483473270d2ef088d3dff15e`  
		Last Modified: Mon, 26 Jul 2021 23:32:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb51b81ac58de42ed99cb933e19ea4d587540a1e741f3480d83cf24a6f47e808`  
		Last Modified: Mon, 26 Jul 2021 23:33:37 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbdb84aef2b635045a5ab08db3a4c76df503b012cf832199476f635ebeff376`  
		Last Modified: Mon, 26 Jul 2021 23:33:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd21a126c78a24237436baa606a4c7a22906a2b13943308b364af25e65afa4f9`  
		Last Modified: Wed, 04 Aug 2021 23:41:54 GMT  
		Size: 129.9 MB (129915575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe83a3a55505f225914d3d42ceaef075e348540616bdf08b564776ccc63a01b`  
		Last Modified: Wed, 04 Aug 2021 23:41:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcf79974a03882a8bb61150c591d60a7fc3a465e479aec5325f9065ddf9fcae`  
		Last Modified: Wed, 04 Aug 2021 23:41:36 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
