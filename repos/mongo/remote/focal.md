## `mongo:focal`

```console
$ docker pull mongo@sha256:b74551ad2bc6479a29cc0bb3ac3a27b27d987f7f76da0ad27c0eba299db632e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:focal` - linux; amd64

```console
$ docker pull mongo@sha256:6a8f5158e1cc05d7bf5a9e6ba9e425a2088073fa397a36a6bd05f8da2ec9667b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.4 MB (231375615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d307892c0b566f5d4548037c3b3cfab58d0b3ccf32c3ddfe921fea84122293f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:30:41 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 02 Aug 2022 20:30:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:30:50 GMT
ENV GOSU_VERSION=1.12
# Tue, 02 Aug 2022 20:30:50 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 02 Aug 2022 20:31:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 20:31:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 24 Aug 2022 23:37:16 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '39BD841E4BE5FB195A65400E6A26B1AE64C3C388'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Wed, 24 Aug 2022 23:37:16 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 24 Aug 2022 23:37:16 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 24 Aug 2022 23:37:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 24 Aug 2022 23:37:16 GMT
ENV MONGO_MAJOR=6.0
# Wed, 24 Aug 2022 23:37:17 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 24 Aug 2022 23:37:17 GMT
ENV MONGO_VERSION=6.0.1
# Wed, 24 Aug 2022 23:37:46 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 24 Aug 2022 23:37:47 GMT
VOLUME [/data/db /data/configdb]
# Wed, 24 Aug 2022 23:37:47 GMT
ENV HOME=/data/db
# Wed, 24 Aug 2022 23:37:47 GMT
COPY file:dbe4d288873410e7437b08aca015eb28310000d0fd3e6f7b112e517db691051e in /usr/local/bin/ 
# Wed, 24 Aug 2022 23:37:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:37:48 GMT
EXPOSE 27017
# Wed, 24 Aug 2022 23:37:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016bc871e2b33f0e2a37272769ebd6defdb4b702f0d41ec1e685f0366b64e64a`  
		Last Modified: Tue, 02 Aug 2022 20:33:16 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddd649edd82d79ffc6f573cd5da7909ae50596b95aca684a571aff6e36aa8cb`  
		Last Modified: Tue, 02 Aug 2022 20:33:17 GMT  
		Size: 3.1 MB (3059542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bf776c01e412c9cf35ea7a41f97370c486dee27a2aab228cf2e850a8863e8b`  
		Last Modified: Tue, 02 Aug 2022 20:33:17 GMT  
		Size: 6.5 MB (6506025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f0405a2fe343547a60a9d4182261ca02d70bb9e47d6cd248f3285d6b41e64c`  
		Last Modified: Tue, 02 Aug 2022 20:33:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89785d0d9c65afe73fbd9bcb29c451090ca84df0e128cf1ecf5712c036e8c9d2`  
		Last Modified: Wed, 24 Aug 2022 23:38:33 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd40d84c80b0302ca13faab8210d8c7082814f6f2ab576b3a61f467d03e1cb0b`  
		Last Modified: Wed, 24 Aug 2022 23:38:33 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50d65ac4752500ab9f3c24c86b4aa218bea9a0bb0a837ae54ffe2e6d2454f5a`  
		Last Modified: Wed, 24 Aug 2022 23:39:00 GMT  
		Size: 193.2 MB (193228772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0068aeddeed2bee4f30c759e840262a4034fabaafda79bdf86a0a85c36d4d`  
		Last Modified: Wed, 24 Aug 2022 23:38:33 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ce28516e0ddbb2b9545623e76fbc3672ba8ab94a63401ac0ace9a2d5008240fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.6 MB (224590078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13501e64d58f6bec45558075e7442fe89cc15642b5704d7db1c0d04a7c345892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:46:08 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 02 Aug 2022 18:46:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:46:42 GMT
ENV GOSU_VERSION=1.12
# Tue, 02 Aug 2022 18:46:43 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 02 Aug 2022 18:47:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:47:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 25 Aug 2022 00:05:57 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '39BD841E4BE5FB195A65400E6A26B1AE64C3C388'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Thu, 25 Aug 2022 00:05:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 25 Aug 2022 00:05:59 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 25 Aug 2022 00:06:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 25 Aug 2022 00:06:01 GMT
ENV MONGO_MAJOR=6.0
# Thu, 25 Aug 2022 00:06:02 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 25 Aug 2022 00:06:03 GMT
ENV MONGO_VERSION=6.0.1
# Thu, 25 Aug 2022 00:06:26 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 25 Aug 2022 00:06:27 GMT
VOLUME [/data/db /data/configdb]
# Thu, 25 Aug 2022 00:06:27 GMT
ENV HOME=/data/db
# Thu, 25 Aug 2022 00:06:29 GMT
COPY file:dbe4d288873410e7437b08aca015eb28310000d0fd3e6f7b112e517db691051e in /usr/local/bin/ 
# Thu, 25 Aug 2022 00:06:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 00:06:30 GMT
EXPOSE 27017
# Thu, 25 Aug 2022 00:06:31 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f92e7525120387a6bc9ec42b9ebfc8115309ab70f65a766e3fda1239d787f9`  
		Last Modified: Tue, 02 Aug 2022 18:51:20 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdda1347325980782ee9b7c6232d712c262b77bc097f712508cf17423dea0de`  
		Last Modified: Tue, 02 Aug 2022 18:51:21 GMT  
		Size: 2.9 MB (2907020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e02463a0f47d7c309281cbc5b4603815ec64c4653d4ed4ac37a06e6bb91b8e`  
		Last Modified: Tue, 02 Aug 2022 18:51:21 GMT  
		Size: 6.2 MB (6249317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9bc5b0968e9dc0079b9ed64930bcf14f8d69847b72f526a1dd1c8bd43df8cc`  
		Last Modified: Tue, 02 Aug 2022 18:51:18 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2908ff18ddc6a5d8953c967541541e6d401812961170bff48186d0847f9c13d3`  
		Last Modified: Thu, 25 Aug 2022 00:08:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966857d017e4236793227a8b33a78aab26fe08ce8ef7741e219ebe0854f4e70b`  
		Last Modified: Thu, 25 Aug 2022 00:08:01 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691117dd4546dbb52bbbbf3aa3bb25da617a11d6f5d26952e103b31232b8d7a1`  
		Last Modified: Thu, 25 Aug 2022 00:08:28 GMT  
		Size: 188.2 MB (188233402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66015fcdb16116a4aa0f39c4e9bbca1ef2bf8b5bdc585345fa8aeb809cbc13d3`  
		Last Modified: Thu, 25 Aug 2022 00:08:01 GMT  
		Size: 5.0 KB (4985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
