## `mongo:focal`

```console
$ docker pull mongo@sha256:e73fd974e3917d543ae3d227a9b43b1abec7b52e1a6088f69e877d25d1f2f5d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:focal` - linux; amd64

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

### `mongo:focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:add6da48a188a4f979c1b99e6f1e2baa746b4fbdd42ff5d176d45de97d48d448
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239484798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:addfd455919fa552fae7dc3cfd6d8fa690c784f7bf07aeaa866e5c87ab106063`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:06:06 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 16 Oct 2021 02:06:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:06:15 GMT
ENV GOSU_VERSION=1.12
# Sat, 16 Oct 2021 02:06:16 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 16 Oct 2021 02:06:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 02:06:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 02:06:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 02:06:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 16 Oct 2021 02:06:45 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 16 Oct 2021 02:06:46 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 16 Oct 2021 02:06:47 GMT
ENV MONGO_MAJOR=5.0
# Sat, 16 Oct 2021 02:06:48 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 16 Oct 2021 02:06:49 GMT
ENV MONGO_VERSION=5.0.3
# Sat, 16 Oct 2021 02:07:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 16 Oct 2021 02:07:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 16 Oct 2021 02:07:12 GMT
VOLUME [/data/db /data/configdb]
# Sat, 16 Oct 2021 02:07:14 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Sat, 16 Oct 2021 02:07:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 02:07:15 GMT
EXPOSE 27017
# Sat, 16 Oct 2021 02:07:16 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b19666caec16fe4ae329c791ac93b397bbc78b9f84cb6e735d21b83b2eb9c0e`  
		Last Modified: Sat, 16 Oct 2021 02:11:19 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7b1addf2da74eccff510de6aa5ab3d3d000656817b97884d02f892fb93248a`  
		Last Modified: Sat, 16 Oct 2021 02:11:19 GMT  
		Size: 2.9 MB (2911827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef180f0d597c6eed96a83a2f6d97d4345b9909ebbee8ac80b5ecc71a368d23b`  
		Last Modified: Sat, 16 Oct 2021 02:11:20 GMT  
		Size: 6.2 MB (6248421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6d24c0ec70825ca68ce4d4304ca3d41b4d65622f2c1758be2423bc43e5b3d`  
		Last Modified: Sat, 16 Oct 2021 02:11:19 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346d14d0731950cdc142603e6f36a1a1f88862b63bfbca743f453854687c6d25`  
		Last Modified: Sat, 16 Oct 2021 02:11:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c6a1451b8d8b9cded5ff44f9960282c4072f710a83595c62fc6778da82bb02`  
		Last Modified: Sat, 16 Oct 2021 02:11:17 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68748565d9e0d7cff2e11e0e2920c28476b051004b142f623dfd774b7c5e3374`  
		Last Modified: Sat, 16 Oct 2021 02:11:43 GMT  
		Size: 203.1 MB (203145319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7832c0e6bbd861db05e9e2017dcecd553ba04004ea2a7c0d4e02af1aac6851ff`  
		Last Modified: Sat, 16 Oct 2021 02:11:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6468d66f0471f9c6d1bb37fda98f07757e8d839a49f24450a4b29c8f83aeea33`  
		Last Modified: Sat, 16 Oct 2021 02:11:17 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
