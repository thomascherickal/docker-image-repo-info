## `mongo:4-focal`

```console
$ docker pull mongo@sha256:05c9988ee6ee4e6009546a13aff7bec208b03724667d66ae0646630753c15487
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4-focal` - linux; amd64

```console
$ docker pull mongo@sha256:68fa51fe8d1108e7b0f650862f26625744be95343315296137bdf2f380526af6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.2 MB (175174001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efbd72d3ba64025b5ee74b2c3ff71967ce30d10f4343c60ea5060c85437346a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:32:20 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 07 Jun 2022 00:32:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:32:28 GMT
ENV GOSU_VERSION=1.12
# Tue, 07 Jun 2022 00:32:28 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 07 Jun 2022 00:32:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:32:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:33:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Tue, 07 Jun 2022 00:33:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Tue, 07 Jun 2022 00:33:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Tue, 07 Jun 2022 00:33:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Tue, 07 Jun 2022 00:33:19 GMT
ENV MONGO_MAJOR=4.4
# Tue, 07 Jun 2022 00:33:20 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 07 Jun 2022 00:33:20 GMT
ENV MONGO_VERSION=4.4.14
# Mon, 13 Jun 2022 22:09:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 13 Jun 2022 22:09:21 GMT
VOLUME [/data/db /data/configdb]
# Mon, 13 Jun 2022 22:09:22 GMT
ENV HOME=/data/db
# Mon, 13 Jun 2022 22:09:22 GMT
COPY file:b7b44e96082c97da2e7f6248f8bbb2edd837542169af52bcc3f53a0cf8b74b7e in /usr/local/bin/ 
# Mon, 13 Jun 2022 22:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Jun 2022 22:09:22 GMT
EXPOSE 27017
# Mon, 13 Jun 2022 22:09:22 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ef66a8492a7b4b656a9dddda9f1bfa3bd3213773c8449b68dadac55605c96f`  
		Last Modified: Tue, 07 Jun 2022 00:34:56 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cec14c8f9e0886403900a1569d2a6a4c33fa3b3984d7dc128eb71c437fe06d`  
		Last Modified: Tue, 07 Jun 2022 00:34:57 GMT  
		Size: 3.1 MB (3064245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c3018eb09a584362cfe9d340566fb755597b453ea58bf5c6c15c8e120efe44`  
		Last Modified: Tue, 07 Jun 2022 00:34:57 GMT  
		Size: 6.5 MB (6506121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc9e1c2556b202042e54ddafe2ae992d58cd462bd3a75ab2c55ccbc42c76dc9`  
		Last Modified: Tue, 07 Jun 2022 00:34:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf64ffd9ac29baa2374dd16340b9f49b854968fc1d658682f9845f629a3193`  
		Last Modified: Tue, 07 Jun 2022 00:35:38 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e2345b80071fb50d8d7defa6cae54cf628c1ff93542632bc9194a082987381`  
		Last Modified: Tue, 07 Jun 2022 00:35:38 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200f27e7d2fd397cd75b9f51a956772e0a7d4eda48040136385ed6f45e043c79`  
		Last Modified: Mon, 13 Jun 2022 22:12:41 GMT  
		Size: 137.0 MB (137022366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6786d2b6ba55564b0440a53468ca6c273c172dfd54bb67b2ae694d2d596fe14`  
		Last Modified: Mon, 13 Jun 2022 22:12:23 GMT  
		Size: 5.0 KB (4951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fd39fd5e9dddb19289bb4da1d77c7a3c36722d94d5d8b1bace8a702110b3643d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.8 MB (166785311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94160a76d7ce38d6fe4cf0efdc2b8b8749a1d88fe31bd80e408d24c1fe901eff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:32:37 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 07 Jun 2022 05:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:32:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 07 Jun 2022 05:32:49 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 07 Jun 2022 05:33:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 05:33:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 05:33:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Tue, 07 Jun 2022 05:33:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Tue, 07 Jun 2022 05:33:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Tue, 07 Jun 2022 05:33:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Tue, 07 Jun 2022 05:33:56 GMT
ENV MONGO_MAJOR=4.4
# Tue, 07 Jun 2022 05:33:57 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 07 Jun 2022 05:33:58 GMT
ENV MONGO_VERSION=4.4.14
# Tue, 07 Jun 2022 05:34:14 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 07 Jun 2022 05:34:14 GMT
VOLUME [/data/db /data/configdb]
# Tue, 07 Jun 2022 05:34:15 GMT
ENV HOME=/data/db
# Tue, 07 Jun 2022 05:34:17 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Tue, 07 Jun 2022 05:34:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 05:34:18 GMT
EXPOSE 27017
# Tue, 07 Jun 2022 05:34:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a81ecfaf7e285e515a2a8a3d6eb9d5f8a5880977cf83c0f2f57c225eae077`  
		Last Modified: Tue, 07 Jun 2022 05:36:25 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cf8516df40b7af9c5365fce0d7792d81cf4b99e78adeb344f70d7d1bbdea02`  
		Last Modified: Tue, 07 Jun 2022 05:36:26 GMT  
		Size: 2.9 MB (2912129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4334b4723aa2cd27affebea50dd246ce909a2f659276d99e1a8126bdb851aa38`  
		Last Modified: Tue, 07 Jun 2022 05:36:26 GMT  
		Size: 6.2 MB (6248751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890407c6615160414ea3572733aa6d67486988daf87eeff669232e7fa3afab5a`  
		Last Modified: Tue, 07 Jun 2022 05:36:23 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef82e8eb9fa451f400ec6e3f1fc17fc17617921bbd1d7a13f82923efe494d95`  
		Last Modified: Tue, 07 Jun 2022 05:37:07 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b6b9a2898f9c514fc6af25b6d44a046eae9f86bc575e050c342654c10e9d8e`  
		Last Modified: Tue, 07 Jun 2022 05:37:07 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e902cddd1f7dbc5a7e04eb203f32d3597766c4592b04cad15608e0a3734f7334`  
		Last Modified: Tue, 07 Jun 2022 05:37:24 GMT  
		Size: 130.4 MB (130424720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f814b656c6a2b68ea3c0ce2f8089d651ed2cb897558081e9eb0c77ec72cb6dd9`  
		Last Modified: Tue, 07 Jun 2022 05:37:07 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
