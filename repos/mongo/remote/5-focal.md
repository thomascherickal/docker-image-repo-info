## `mongo:5-focal`

```console
$ docker pull mongo@sha256:6724982f0ac9c4e25c8a35272d6aca00d9d08fc249988138c4ac05292aa62c62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:5-focal` - linux; amd64

```console
$ docker pull mongo@sha256:b19536b990ba5542c868ec34bfdea4b96d608de6908281de5253df4fb3422532
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.7 MB (249706676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20106db9aa7ac731551a17d6ec07e61fb442221460e5106fa70be71d98b5ee85`
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
# Fri, 22 Apr 2022 04:22:13 GMT
ENV MONGO_VERSION=5.0.7
# Fri, 22 Apr 2022 04:22:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 22 Apr 2022 04:22:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 22 Apr 2022 04:22:54 GMT
VOLUME [/data/db /data/configdb]
# Fri, 22 Apr 2022 04:22:54 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Fri, 22 Apr 2022 04:22:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 04:22:55 GMT
EXPOSE 27017
# Fri, 22 Apr 2022 04:22:55 GMT
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
	-	`sha256:8a2fd96bceb84a1062d419914c6ddb4497c0c05c6301038ae687084c80961349`  
		Last Modified: Fri, 22 Apr 2022 04:26:36 GMT  
		Size: 211.6 MB (211562246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f784c3fad6f75a71f2f1a5d482596b40e2722481820d2e8da14796bcb8e1a2`  
		Last Modified: Fri, 22 Apr 2022 04:26:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907cb14703af1351c0186953bfd7e16192fb73ee706a37b376842466356cc978`  
		Last Modified: Fri, 22 Apr 2022 04:26:06 GMT  
		Size: 4.9 KB (4949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:27d23086fdbe0200178e2c19cc53673a126e8e6971dcb098ea91a81bfe91f11e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241849053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ee9200a31b09e14e5c37ed0351f6a35da0f97dc33b6ca53da4882c308a2b7e`
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
# Fri, 22 Apr 2022 03:41:06 GMT
ENV MONGO_VERSION=5.0.7
# Fri, 22 Apr 2022 03:41:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 22 Apr 2022 03:41:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 22 Apr 2022 03:41:30 GMT
VOLUME [/data/db /data/configdb]
# Fri, 22 Apr 2022 03:41:32 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Fri, 22 Apr 2022 03:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 03:41:33 GMT
EXPOSE 27017
# Fri, 22 Apr 2022 03:41:34 GMT
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
	-	`sha256:6442d9c5c4916fc3a7fcfc29b917c1c43ecf5529032bab431867877bc087df88`  
		Last Modified: Fri, 22 Apr 2022 03:46:15 GMT  
		Size: 205.5 MB (205511760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e0510e15822ac3accf3451fbd4fb194a00b3125a01ed34c69ae595315ae63c`  
		Last Modified: Fri, 22 Apr 2022 03:45:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece99e6e5857ec251d278410fd78b7efcb8e774418bf20851e3d7c8860b96def`  
		Last Modified: Fri, 22 Apr 2022 03:45:48 GMT  
		Size: 5.0 KB (4951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
