## `mongo:focal`

```console
$ docker pull mongo@sha256:8cf855aa70f59dcc95062a649db9278697006097b277e59c6fb574f2157a0b50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:focal` - linux; amd64

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

### `mongo:focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8bf4699bcceef7f928e15f8399a3b6cf904068c669001f99f18b7b9b3efb7959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241913249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8545a6005ade67bbc163ceb1beef35e796e9069a6db1cf478cda8a3e8152236a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:40:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 22 Apr 2022 03:40:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:40:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 03:40:42 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 22 Apr 2022 03:40:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 03:40:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 03:41:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Fri, 22 Apr 2022 03:41:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 22 Apr 2022 03:41:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 22 Apr 2022 03:41:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 22 Apr 2022 03:41:04 GMT
ENV MONGO_MAJOR=5.0
# Fri, 22 Apr 2022 03:41:05 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 Apr 2022 00:40:09 GMT
ENV MONGO_VERSION=5.0.8
# Wed, 27 Apr 2022 00:40:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 Apr 2022 00:40:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 Apr 2022 00:40:32 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 Apr 2022 00:40:34 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Wed, 27 Apr 2022 00:40:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Apr 2022 00:40:35 GMT
EXPOSE 27017
# Wed, 27 Apr 2022 00:40:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7656e31ac835898115bb062417518da45f13d844d45b113a3e0ec052fb7ed5`  
		Last Modified: Fri, 22 Apr 2022 03:45:51 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9afb565f40abd7917924ee0c971fde0ca8af95d6f59c86f58ea3ac8ec9ad7f`  
		Last Modified: Fri, 22 Apr 2022 03:45:52 GMT  
		Size: 2.9 MB (2911515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6479c288bbabe768e64609b13c00107f5646915d271aef379d57590b5ddaec96`  
		Last Modified: Fri, 22 Apr 2022 03:45:52 GMT  
		Size: 6.2 MB (6248046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2408809f3c6264deca9ff994596548daac089ba5f9867a86450b79f9b3535b38`  
		Last Modified: Fri, 22 Apr 2022 03:45:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2ea3e4ddfa1782f37cd67f8dd624f44c11a3f205370c8d0fce2b433cf00ba6`  
		Last Modified: Fri, 22 Apr 2022 03:45:48 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c918d4dbc757e126532f3a3b31c7f69af566975701ff01229ea429ba0c7ddf4d`  
		Last Modified: Fri, 22 Apr 2022 03:45:48 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4583777ee71b232de7e49e18d7b1c35358f8114dfa732841763018431f4080`  
		Last Modified: Wed, 27 Apr 2022 00:42:30 GMT  
		Size: 205.6 MB (205575958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb72c771fdb0a610ee88abeb3ecc584d8e78f5cd1002fe5552b90fe28e7f08e`  
		Last Modified: Wed, 27 Apr 2022 00:42:03 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4689bf2796435ba8b16ac886ad484fe99adcceab7d5325ba5796f849530809ca`  
		Last Modified: Wed, 27 Apr 2022 00:42:03 GMT  
		Size: 4.9 KB (4949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
