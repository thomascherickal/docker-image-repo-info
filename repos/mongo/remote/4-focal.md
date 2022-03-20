## `mongo:4-focal`

```console
$ docker pull mongo@sha256:723a7724dbe9574c997fa1e221c2fa5e8b5d9e84757ba3f71f7378fd1462456d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4-focal` - linux; amd64

```console
$ docker pull mongo@sha256:2a0e4529f71b3d5c0b1012b2063ecd64793350438865db60ed9256f904e0931a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.7 MB (171671340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd8d12514c6b08a97d8f79449e3db862a571f9dd2efff6673401831a24e0e0aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 23:10:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 19 Mar 2022 23:10:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 23:10:48 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:10:48 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 19 Mar 2022 23:10:59 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:10:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 19 Mar 2022 23:12:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Sat, 19 Mar 2022 23:12:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 19 Mar 2022 23:12:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 19 Mar 2022 23:12:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 19 Mar 2022 23:12:24 GMT
ENV MONGO_MAJOR=4.4
# Sat, 19 Mar 2022 23:12:24 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 19 Mar 2022 23:12:24 GMT
ENV MONGO_VERSION=4.4.13
# Sat, 19 Mar 2022 23:12:42 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 19 Mar 2022 23:12:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 19 Mar 2022 23:12:43 GMT
VOLUME [/data/db /data/configdb]
# Sat, 19 Mar 2022 23:12:43 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Sat, 19 Mar 2022 23:12:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:12:43 GMT
EXPOSE 27017
# Sat, 19 Mar 2022 23:12:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a89ffa9c8eced01a2f48049d85ae168acd7a60f7ac623fefe24f267e8a63f4`  
		Last Modified: Sat, 19 Mar 2022 23:14:15 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a26a1adeb957c889480f9697a2b513d2a16eb6b988a5b9b677c78852d2ac26`  
		Last Modified: Sat, 19 Mar 2022 23:14:16 GMT  
		Size: 3.1 MB (3064036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c4ca429ae25b7556df4d0c248f248941deb11000995ffed150884bc69464c`  
		Last Modified: Sat, 19 Mar 2022 23:14:17 GMT  
		Size: 6.5 MB (6505671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd51bf7ebc1976b11f5b2b7aaca84c7f74fd7017e55503fcc027cdb0be329b`  
		Last Modified: Sat, 19 Mar 2022 23:14:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15136b3b3dc8dbb3531835b61c74a52dde2bae01fddd6cc83bacab5d2d8de51`  
		Last Modified: Sat, 19 Mar 2022 23:14:57 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c41ea5e7608b815d5be5b8531524880c516cec4df44854a05f8ce180d54289`  
		Last Modified: Sat, 19 Mar 2022 23:14:57 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1243afbc143dc04dae2a2325fc0fe822a5cc99264e308adc35d3b099c36ec042`  
		Last Modified: Sat, 19 Mar 2022 23:15:15 GMT  
		Size: 133.5 MB (133527003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a81d9de0fd7b1a2083e071f71223e9e382a89d3e2ea20e7380e72101471f11d`  
		Last Modified: Sat, 19 Mar 2022 23:14:57 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d895b406e4e5c57c18ea2fd5372967da20948f1f8b6457bb2b6a0df97e772920`  
		Last Modified: Sat, 19 Mar 2022 23:14:57 GMT  
		Size: 4.9 KB (4945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:6b12ab969eceb39279a1be3ec720b3be7e99600d1cae69fb515b079904deb816
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.8 MB (166757188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97c66ce4931dd4327246bcd4a8def286323e3eb9ab14baf20354a6c99c27506b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:59:32 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 19 Mar 2022 15:59:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:59:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 15:59:44 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 19 Mar 2022 15:59:59 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 16:00:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 19 Mar 2022 16:02:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Sat, 19 Mar 2022 16:02:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 19 Mar 2022 16:02:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 19 Mar 2022 16:02:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 19 Mar 2022 16:02:09 GMT
ENV MONGO_MAJOR=4.4
# Sat, 19 Mar 2022 16:02:10 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 19 Mar 2022 16:02:11 GMT
ENV MONGO_VERSION=4.4.13
# Sat, 19 Mar 2022 16:02:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 19 Mar 2022 16:02:28 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 19 Mar 2022 16:02:29 GMT
VOLUME [/data/db /data/configdb]
# Sat, 19 Mar 2022 16:02:31 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Sat, 19 Mar 2022 16:02:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 16:02:32 GMT
EXPOSE 27017
# Sat, 19 Mar 2022 16:02:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b19f2c434348a5db704ae793be9e303aed49d7cb6edc8420bf0795e0cdc8b58`  
		Last Modified: Sat, 19 Mar 2022 16:05:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c540312e67d90471a980e2e48aacd2573c06a3bf93af280772ae08b32728e41`  
		Last Modified: Sat, 19 Mar 2022 16:05:24 GMT  
		Size: 2.9 MB (2911889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641aafb779d3f584e9519ba8d8dcbdb535081b8557255b5e432cc7d94a0d96e6`  
		Last Modified: Sat, 19 Mar 2022 16:05:24 GMT  
		Size: 6.2 MB (6248279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb3d117525b084e74c1493f4094b1db20709b3d8a5d3690a97f5340287e0d0c`  
		Last Modified: Sat, 19 Mar 2022 16:05:23 GMT  
		Size: 112.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa44b48049dfa9b8118a2310fcef7f54140c803756c675bc4c607a5c9131e49`  
		Last Modified: Sat, 19 Mar 2022 16:06:08 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13ecc04e1c70e844f4bac36dc1b7552b919ee2e89e4f2c9a659a9faab81d6c7`  
		Last Modified: Sat, 19 Mar 2022 16:06:08 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e7c0108d710517e4dd53862a87c26ca141af26662256679bed5e3654fb9cdb`  
		Last Modified: Sat, 19 Mar 2022 16:06:25 GMT  
		Size: 130.4 MB (130418819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18342683b0232bb65366c1a2bdb060c6e955aa1576aba72a3366a8e33a8bba39`  
		Last Modified: Sat, 19 Mar 2022 16:06:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760a19c16557a3f193f021b57bbf9abad2b5395f5527971190fab01558c0640b`  
		Last Modified: Sat, 19 Mar 2022 16:06:08 GMT  
		Size: 4.9 KB (4947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
