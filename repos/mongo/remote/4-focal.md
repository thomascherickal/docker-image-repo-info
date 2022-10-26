## `mongo:4-focal`

```console
$ docker pull mongo@sha256:36f1610f211d226bc472c28b67d2da64ad3294cb1439149dcb3e22cbdbc26c5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4-focal` - linux; amd64

```console
$ docker pull mongo@sha256:a88d9e1d0bbf6fd4b57f4accc9000b0f3a76b2d9216180788d92956a7437ea0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.8 MB (172837363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dba92ac6108e65933b60e1bd9d03bd8713502d39af6096551c16fe145ca1f807`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:30:12 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 05 Oct 2022 18:30:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:30:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 05 Oct 2022 18:30:20 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 05 Oct 2022 18:30:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 18:30:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 18:31:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Wed, 05 Oct 2022 18:31:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 05 Oct 2022 18:31:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 05 Oct 2022 18:31:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 05 Oct 2022 18:31:44 GMT
ENV MONGO_MAJOR=4.4
# Wed, 05 Oct 2022 18:31:45 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 05 Oct 2022 18:31:45 GMT
ENV MONGO_VERSION=4.4.17
# Wed, 05 Oct 2022 18:32:03 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 05 Oct 2022 18:32:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 05 Oct 2022 18:32:04 GMT
ENV HOME=/data/db
# Wed, 05 Oct 2022 18:32:05 GMT
COPY file:a062061dd38363517a589afdd763f61500b162faee89d415017c58fd70abe392 in /usr/local/bin/ 
# Wed, 05 Oct 2022 18:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:32:05 GMT
EXPOSE 27017
# Wed, 05 Oct 2022 18:32:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81bcd64a2d26fbd2741700cc3f6f1aa783ae202298d8010aca8c60f034c4e59`  
		Last Modified: Wed, 05 Oct 2022 18:33:32 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ed91f63dfa037fa6061dee8f91d31f24a66375c70d652e8ee3c77e9e20b0fe`  
		Last Modified: Wed, 05 Oct 2022 18:33:33 GMT  
		Size: 3.1 MB (3059535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d1770a2c11d56f4506d0efdc18d345c397565f38270c9f33347a483a8bfb58`  
		Last Modified: Wed, 05 Oct 2022 18:33:33 GMT  
		Size: 6.5 MB (6505968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d917eab2f0dc57fe40f116099f93a233b75e63df943d2a84d37623faf91ed`  
		Last Modified: Wed, 05 Oct 2022 18:33:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae23fd926d5289d7f9939344270c99e24906888a69783c1d69bfd2cd5d522d60`  
		Last Modified: Wed, 05 Oct 2022 18:34:54 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e23a31f26283ab44fab40c519e3cdf154a2b4f38cd7b70a0cd5772124f39240`  
		Last Modified: Wed, 05 Oct 2022 18:34:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1670c0330a4ef40749c20aa01f2a34e2b097b637f93d81f30572450696cb32`  
		Last Modified: Wed, 05 Oct 2022 18:35:12 GMT  
		Size: 134.7 MB (134688648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e00f823fe51d15240f771d361ef692401c41aa1a69881afbcb4bfe81cf8fa6`  
		Last Modified: Wed, 05 Oct 2022 18:34:54 GMT  
		Size: 5.1 KB (5069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:9becb9445342861fa6364d4ed1342ae4530ef1229a5fda54e42f609391065e54
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167854667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632b583ce348265859e875db8be95ba7d58129837fedd533f074d81901521bce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:12:08 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 26 Oct 2022 02:12:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:12:16 GMT
ENV GOSU_VERSION=1.12
# Wed, 26 Oct 2022 02:12:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 26 Oct 2022 02:12:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:12:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:13:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Wed, 26 Oct 2022 02:13:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 26 Oct 2022 02:13:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 26 Oct 2022 02:13:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 26 Oct 2022 02:13:25 GMT
ENV MONGO_MAJOR=4.4
# Wed, 26 Oct 2022 02:13:25 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 26 Oct 2022 02:13:25 GMT
ENV MONGO_VERSION=4.4.17
# Wed, 26 Oct 2022 02:13:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 26 Oct 2022 02:13:40 GMT
VOLUME [/data/db /data/configdb]
# Wed, 26 Oct 2022 02:13:40 GMT
ENV HOME=/data/db
# Wed, 26 Oct 2022 02:13:40 GMT
COPY file:a062061dd38363517a589afdd763f61500b162faee89d415017c58fd70abe392 in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:13:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:13:40 GMT
EXPOSE 27017
# Wed, 26 Oct 2022 02:13:40 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffac05d305dafc7bd6d968c4d611342ceb95a87494c361ab37718b188f02763`  
		Last Modified: Wed, 26 Oct 2022 02:16:20 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d44feb31079d0e2421a83a8dd5563d203ec1ff537396d3ed65dd35cdfed206f`  
		Last Modified: Wed, 26 Oct 2022 02:16:21 GMT  
		Size: 2.9 MB (2907461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd79df0bf56efa1ec22177052bd5d6e4feef423ad95176bd0f86a478f3f99d30`  
		Last Modified: Wed, 26 Oct 2022 02:16:21 GMT  
		Size: 6.4 MB (6425791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393c4defd29fb265c4d4794d5f008fbde7c8d9c4f91a7105e9cf2866a28df77a`  
		Last Modified: Wed, 26 Oct 2022 02:16:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9543ed4a0c19afac9cad8f19103e2829189e0fa876644e0e6ce17ecc220cb9`  
		Last Modified: Wed, 26 Oct 2022 02:17:27 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef78c2204a4b9c23f0f0cfdc6569879d599a4367241d590f3f289f5353629b31`  
		Last Modified: Wed, 26 Oct 2022 02:17:27 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379f78d03cd7ee2f44a57261c3ab81c0c71ba6cce08f4d39284836ed59445f15`  
		Last Modified: Wed, 26 Oct 2022 02:17:39 GMT  
		Size: 131.3 MB (131316654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed0f1ddf3fc5fc50039ddfcc2301fc5cb3ee1005b1bc53d3ac54290bec84c9c`  
		Last Modified: Wed, 26 Oct 2022 02:17:27 GMT  
		Size: 5.1 KB (5070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
