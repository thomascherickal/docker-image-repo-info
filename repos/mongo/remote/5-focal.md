## `mongo:5-focal`

```console
$ docker pull mongo@sha256:2a3cb18fb479d38a9b889d3529188b45a469e0f2ac8d222da1eb259273030ec6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:5-focal` - linux; amd64

```console
$ docker pull mongo@sha256:ecff39e98f16fbd0de6c74eb56967cf26e1443c1ee1383fdae67f04d427e2aa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249766521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7babdf608274b5cb26dd6bdd790fa42b229e44aac808c537e091efc7933ecca4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:21:52 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 22 Apr 2022 04:22:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:22:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 04:22:00 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 22 Apr 2022 04:22:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 04:22:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 04:22:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Fri, 22 Apr 2022 04:22:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 22 Apr 2022 04:22:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 22 Apr 2022 04:22:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 22 Apr 2022 04:22:12 GMT
ENV MONGO_MAJOR=5.0
# Fri, 22 Apr 2022 04:22:13 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 Apr 2022 00:25:50 GMT
ENV MONGO_VERSION=5.0.8
# Wed, 27 Apr 2022 00:26:25 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 Apr 2022 00:26:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 Apr 2022 00:26:27 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 Apr 2022 00:26:27 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Wed, 27 Apr 2022 00:26:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Apr 2022 00:26:27 GMT
EXPOSE 27017
# Wed, 27 Apr 2022 00:26:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3a1df854b89f41965414e9ddb9ed1135bd13e15b256e733bae8aac6b7c63e1`  
		Last Modified: Fri, 22 Apr 2022 04:26:09 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0a2dae0995ae0954b8776744eaa7043aafcc171cade65b8c746ed4f122716a`  
		Last Modified: Fri, 22 Apr 2022 04:26:09 GMT  
		Size: 3.1 MB (3064031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a418b0c4e4fa5cae1cd4e02c0904ee6d76e5117ad1c3fc24796e57308f82c7a8`  
		Last Modified: Fri, 22 Apr 2022 04:26:10 GMT  
		Size: 6.5 MB (6505681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5ea9c2d40e2e3a9dbd454c60488c94f8820f317fc92a7b68e70b3e5a251309`  
		Last Modified: Fri, 22 Apr 2022 04:26:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f494f5d4b55ac70efcbc6bbd962daa42b3e1cc86a15ee6cce2fe803c898d7e49`  
		Last Modified: Fri, 22 Apr 2022 04:26:06 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b969a6b5e7556ae2ff6056979f224b978bdea9bb31e66b644064d438c8d4ea20`  
		Last Modified: Fri, 22 Apr 2022 04:26:06 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a92e6baaae41317d800edcce07552cad372eb44f523a8a9e2d25178001875`  
		Last Modified: Wed, 27 Apr 2022 00:27:39 GMT  
		Size: 211.6 MB (211622089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c44fa8dc96bbbe0aff8f23874dc1f8631a95ef66176761a9a1b603813c4daa`  
		Last Modified: Wed, 27 Apr 2022 00:27:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168667f55eef63bc5a2ec10630ff07d2ae23b25d247d197ad65f90c5f0bde5ee`  
		Last Modified: Wed, 27 Apr 2022 00:27:10 GMT  
		Size: 5.0 KB (4950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e17c2c502c1e3cf1c39f5eb74f73035566e733418684b88c4483cf004654ac3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241914194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b7803cb64be9343a9e08cb81e3dd6d6557e8aeb08344e5ac94aa4bb521897af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:59:39 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 30 Apr 2022 00:59:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:59:49 GMT
ENV GOSU_VERSION=1.12
# Sat, 30 Apr 2022 00:59:50 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 30 Apr 2022 01:00:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:00:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:00:08 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Sat, 30 Apr 2022 01:00:08 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 30 Apr 2022 01:00:09 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 30 Apr 2022 01:00:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 30 Apr 2022 01:00:11 GMT
ENV MONGO_MAJOR=5.0
# Sat, 30 Apr 2022 01:00:12 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 30 Apr 2022 01:00:13 GMT
ENV MONGO_VERSION=5.0.8
# Sat, 30 Apr 2022 01:00:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 30 Apr 2022 01:00:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 30 Apr 2022 01:00:39 GMT
VOLUME [/data/db /data/configdb]
# Sat, 30 Apr 2022 01:00:41 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:00:42 GMT
EXPOSE 27017
# Sat, 30 Apr 2022 01:00:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2905e503bba5cabc836e98f44231192481fc1bbdbb490746f66fe06e85112373`  
		Last Modified: Sat, 30 Apr 2022 01:05:01 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2fbfedcbbd5836fcf2acfd4eb776878244a44f12b71a3c4fb18e285ab7afd1`  
		Last Modified: Sat, 30 Apr 2022 01:05:01 GMT  
		Size: 2.9 MB (2911377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed819c9035120a3b2e0dfddbd0da9c877f71d2ad339de57b514c7c346213475`  
		Last Modified: Sat, 30 Apr 2022 01:05:01 GMT  
		Size: 6.2 MB (6247905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9476a7638d326b957e4885732ba2bb1e87564becc4b674565f8d575a0a60ea`  
		Last Modified: Sat, 30 Apr 2022 01:05:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92607998c5bdd867afc327e0bf70ef2d8704863ab50890eec849201cea43aad9`  
		Last Modified: Sat, 30 Apr 2022 01:04:58 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283d97f7e29f1641ad4b1015a59ce9c61e4b8fe6d61d0f71a7c05b67c8ed982a`  
		Last Modified: Sat, 30 Apr 2022 01:04:58 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef43e52aca7e8b08c4baae40655f463e2aa7599bdfbcd10b7e99b1ca8cdb99c`  
		Last Modified: Sat, 30 Apr 2022 01:05:25 GMT  
		Size: 205.6 MB (205576937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f8fb241d1a1a4e864d328188a6ecb6cce565fd913eeba07bbfc8dc605d306f`  
		Last Modified: Sat, 30 Apr 2022 01:04:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572aa5df790dcf5ff36fea7d838b22bf34174fee6aca97d44f3adb56953ec899`  
		Last Modified: Sat, 30 Apr 2022 01:04:58 GMT  
		Size: 5.0 KB (4951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
