## `mongo:focal`

```console
$ docker pull mongo@sha256:1ceee9ce65425031d09eedcce7033da32ee382d6bec0f047e736d5593a16157b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:focal` - linux; amd64

```console
$ docker pull mongo@sha256:f8b2c5ed1ad675d9b78a3c8f0250c893be5897b5e575a72e1193a9d18212e45f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248874801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:798d1656acbafd5859700cb294bdd1d4b2a0f4fa7f649618a6d842c66aabdb4b`
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
# Sat, 19 Mar 2022 23:11:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Sat, 19 Mar 2022 23:11:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 19 Mar 2022 23:11:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 19 Mar 2022 23:11:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 19 Mar 2022 23:11:31 GMT
ENV MONGO_MAJOR=5.0
# Sat, 19 Mar 2022 23:11:32 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 19 Mar 2022 23:11:32 GMT
ENV MONGO_VERSION=5.0.6
# Sat, 19 Mar 2022 23:11:56 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 19 Mar 2022 23:11:58 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 19 Mar 2022 23:11:58 GMT
VOLUME [/data/db /data/configdb]
# Sat, 19 Mar 2022 23:11:58 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Sat, 19 Mar 2022 23:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:11:58 GMT
EXPOSE 27017
# Sat, 19 Mar 2022 23:11:58 GMT
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
	-	`sha256:68750eb424ec372357002552006c0772867564bfed926a175c6592a5abc715b8`  
		Last Modified: Sat, 19 Mar 2022 23:14:13 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008900bad1d7201ca6a125856033405f3037f95d649cf0d3c01c3ee36865fe10`  
		Last Modified: Sat, 19 Mar 2022 23:14:13 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33eed19868f78eb694319577f423145de02979385c9ee614ba6e4b281c91c16`  
		Last Modified: Sat, 19 Mar 2022 23:14:42 GMT  
		Size: 210.7 MB (210730460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bc3cbfdaeb46ae22b7a06663753debe55d8199b1872a55183e1c110609220e`  
		Last Modified: Sat, 19 Mar 2022 23:14:13 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358eefa21051e7e1cbb086f37ccc98baa3db644cdeaa0b347e724cc3a12ffa79`  
		Last Modified: Sat, 19 Mar 2022 23:14:13 GMT  
		Size: 5.0 KB (4950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:30182ed46dbfbdb7e1d521939f503527b2390fe18a2926b861e3904bfffe3b14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241082508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e4b429a7a59bddc592a16d33c5b2f0bb9c64c1b47dfb63a2901d254b576ab3`
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
# Sat, 19 Mar 2022 16:00:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Sat, 19 Mar 2022 16:00:42 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 19 Mar 2022 16:00:43 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 19 Mar 2022 16:00:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 19 Mar 2022 16:00:45 GMT
ENV MONGO_MAJOR=5.0
# Sat, 19 Mar 2022 16:00:46 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 19 Mar 2022 16:00:47 GMT
ENV MONGO_VERSION=5.0.6
# Sat, 19 Mar 2022 16:01:09 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 19 Mar 2022 16:01:10 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 19 Mar 2022 16:01:11 GMT
VOLUME [/data/db /data/configdb]
# Sat, 19 Mar 2022 16:01:13 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Sat, 19 Mar 2022 16:01:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 16:01:14 GMT
EXPOSE 27017
# Sat, 19 Mar 2022 16:01:15 GMT
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
	-	`sha256:6ea3180b7265b1219124e079529979509b038d2626b9c505e2baaa15eb0aedaa`  
		Last Modified: Sat, 19 Mar 2022 16:05:21 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce835a4ffb7aa0a951248db2451b29b3ede6fccf01ecc1dca8e10d683cafa7a`  
		Last Modified: Sat, 19 Mar 2022 16:05:21 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb815b6451f7d4bf3fd730131f4072136558fda3cf1ec7640371fc5511e1b2a`  
		Last Modified: Sat, 19 Mar 2022 16:05:49 GMT  
		Size: 204.7 MB (204744139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f7c2b17caa13058ec1a2a7bee62c291d65e6d199dc4b1bafaee59a1243f4bf`  
		Last Modified: Sat, 19 Mar 2022 16:05:21 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acabb6372b6f69b7e64509c714c625269bd71f8260eb4d06f3b30c80bd5d71e`  
		Last Modified: Sat, 19 Mar 2022 16:05:21 GMT  
		Size: 5.0 KB (4950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
