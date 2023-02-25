## `mongo:4-focal`

```console
$ docker pull mongo@sha256:df0226b31930eddab66a6e42ed8efd867236e1b82e2cd67f1e58c0fe8c04968f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4-focal` - linux; amd64

```console
$ docker pull mongo@sha256:11da11392f943d25b6dc81ad539f6fc646dd12fcb0e69c11713b06162dd30f5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173178687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec294f2707c5505a08a87d386c4a0b5122a217f7032817d156de3e39026336d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:26:06 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 01 Feb 2023 19:26:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:26:21 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 19:26:21 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 01 Feb 2023 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 19:28:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 19:28:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 01 Feb 2023 19:28:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 01 Feb 2023 19:28:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 01 Feb 2023 19:28:07 GMT
ENV MONGO_MAJOR=4.4
# Wed, 01 Feb 2023 19:28:07 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 25 Feb 2023 00:38:07 GMT
ENV MONGO_VERSION=4.4.19
# Sat, 25 Feb 2023 00:38:24 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 25 Feb 2023 00:38:25 GMT
VOLUME [/data/db /data/configdb]
# Sat, 25 Feb 2023 00:38:25 GMT
ENV HOME=/data/db
# Sat, 25 Feb 2023 00:38:25 GMT
COPY file:82adc06ee9084caf92c64e3fbb536f06b2a724aa0c1f122d17c10c70a5a1b90e in /usr/local/bin/ 
# Sat, 25 Feb 2023 00:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 00:38:25 GMT
EXPOSE 27017
# Sat, 25 Feb 2023 00:38:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7638a79c68d650ad78bf1c04cbc9ef160606e02e19fcdfc357d3a49d9f3dfb`  
		Last Modified: Wed, 01 Feb 2023 19:29:02 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edb8e32447e402814b615208f1a93870bff3994e2b654ae16c438879bc31277`  
		Last Modified: Wed, 01 Feb 2023 19:29:03 GMT  
		Size: 8.3 MB (8348522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b078a16e980d806afa564ded9aaef5b7cf74b44a75880db13e1912297a6bc0c`  
		Last Modified: Wed, 01 Feb 2023 19:29:02 GMT  
		Size: 1.3 MB (1255800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09083ae98273683297e023dfe39760a10a453891715f75c451db8f0916beecd`  
		Last Modified: Wed, 01 Feb 2023 19:29:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eafcd88aa8959f78a0ac45a744a6202992517e3055b4de3b2a436738a02ef88`  
		Last Modified: Wed, 01 Feb 2023 19:30:45 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d81a4f8c99b0b5df00ebf86a6224546c37520ea35bbcd7ddac93281db7292ff`  
		Last Modified: Wed, 01 Feb 2023 19:30:45 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d248a55d605e6cd6939d9bed48f6cc0a219b4b7c47bf3015fd9157eb18f91823`  
		Last Modified: Sat, 25 Feb 2023 00:40:21 GMT  
		Size: 135.0 MB (134987838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bc9dacc663b4045f5f548f82f7a03b91a19cb2445ac05c1bfb330af6910d8c`  
		Last Modified: Sat, 25 Feb 2023 00:40:05 GMT  
		Size: 5.0 KB (4962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:1f597c605bdc2a244e7b58ab9f14abcadf4905c2efe6dbf7b21e7b7267e3bbd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167925984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57484ca2d932d39f6fccb87c0498c93599de3a10bfebd2b5793bb57fd583892f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:03:40 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 01 Feb 2023 19:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:03:55 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 19:03:55 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 01 Feb 2023 19:04:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 19:04:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 19:05:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 19:05:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 01 Feb 2023 19:05:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 01 Feb 2023 19:05:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 01 Feb 2023 19:05:34 GMT
ENV MONGO_MAJOR=4.4
# Wed, 01 Feb 2023 19:05:34 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Feb 2023 23:40:21 GMT
ENV MONGO_VERSION=4.4.19
# Fri, 24 Feb 2023 23:40:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Feb 2023 23:40:36 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Feb 2023 23:40:36 GMT
ENV HOME=/data/db
# Fri, 24 Feb 2023 23:40:36 GMT
COPY file:82adc06ee9084caf92c64e3fbb536f06b2a724aa0c1f122d17c10c70a5a1b90e in /usr/local/bin/ 
# Fri, 24 Feb 2023 23:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Feb 2023 23:40:36 GMT
EXPOSE 27017
# Fri, 24 Feb 2023 23:40:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197e79a593996392dc9c7dea7b4eebe9567f190b13e33b96315e3fa7bfe0cbff`  
		Last Modified: Wed, 01 Feb 2023 19:06:35 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a54d19161368d031ebb2bd8697e5077e32faea13ed42ef3bc01f1521db0b059`  
		Last Modified: Wed, 01 Feb 2023 19:06:36 GMT  
		Size: 8.2 MB (8177815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547f0e899b28966b8bd3a9247256403aacd1bfe5043f9848fabacbfb38ffd92`  
		Last Modified: Wed, 01 Feb 2023 19:06:35 GMT  
		Size: 1.2 MB (1188343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315a8963db2b1f685b9da4bc23fab83cc03ce32eff34be384499607a1416459e`  
		Last Modified: Wed, 01 Feb 2023 19:06:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf4c6bb7f3ac1ee2a96c32dcdc6b80c7c36f3ce9bd58cf37fa5bfea7632879`  
		Last Modified: Wed, 01 Feb 2023 19:07:52 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edbe4572bc8412bb731f1d8bd183b299b9c677afbcb52662976393e4ebd6fa`  
		Last Modified: Wed, 01 Feb 2023 19:07:52 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ca33cbac808e34be02350560c61c7d599fd7c264e22615d23af0933e970424`  
		Last Modified: Fri, 24 Feb 2023 23:42:22 GMT  
		Size: 131.4 MB (131357441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b3f1471d1d08410597ca373685682467ff7fd384e9e1d9f182ae146a2392ba`  
		Last Modified: Fri, 24 Feb 2023 23:42:10 GMT  
		Size: 5.0 KB (4959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
