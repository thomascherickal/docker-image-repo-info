## `mongo:5-focal`

```console
$ docker pull mongo@sha256:39f6992c6f23457ba212f86f226ffa28e15b7b5873602a12e1f6c322901a96e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:5-focal` - linux; amd64

```console
$ docker pull mongo@sha256:27d1b94856d816baba40786ed3412064c939c804a51f8bc6057c3ade301a9c81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254679198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8735eb905a8fba4ff109a7c3b40ff5da6f4e365adbf31427bf3ea179c29393`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:43:43 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 03 May 2023 04:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 04:29:00 GMT
ENV GOSU_VERSION=1.16
# Wed, 03 May 2023 04:29:00 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 03 May 2023 04:29:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 May 2023 04:29:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 May 2023 04:29:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 03 May 2023 04:29:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 03 May 2023 04:29:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 03 May 2023 04:29:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 03 May 2023 04:29:10 GMT
ENV MONGO_MAJOR=5.0
# Wed, 03 May 2023 04:29:11 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 03 May 2023 04:29:11 GMT
ENV MONGO_VERSION=5.0.17
# Wed, 03 May 2023 04:29:40 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 03 May 2023 04:29:41 GMT
VOLUME [/data/db /data/configdb]
# Wed, 03 May 2023 04:29:41 GMT
ENV HOME=/data/db
# Wed, 03 May 2023 04:29:41 GMT
COPY file:e3d6a34db83fe880626bff5d0b8d720ae43720caac9c739cbd1d336a129dad2d in /usr/local/bin/ 
# Wed, 03 May 2023 04:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 04:29:41 GMT
EXPOSE 27017
# Wed, 03 May 2023 04:29:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6653ceb2297789e4fe13aba3af53f096e83ecc4ad4417356ea72e4f9e8b7dccb`  
		Last Modified: Tue, 18 Apr 2023 02:45:51 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e067c5774dde349c4127278bc0f06acc2f6d6a88bff74983171225648b999315`  
		Last Modified: Wed, 03 May 2023 04:32:35 GMT  
		Size: 8.3 MB (8348562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2512535c9bcf2f6101b06b4fe0ed1c287f5468ff706040b190898672771028`  
		Last Modified: Wed, 03 May 2023 04:32:34 GMT  
		Size: 1.3 MB (1255808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95823dd641199b73cc53f548fee010eee561dfe2ebae9a7ee571fe1452e33db0`  
		Last Modified: Wed, 03 May 2023 04:32:31 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806644aafaf1d573325b8e49c6fc90554de5be9e9768cde4f3c7f2c1716ae0ec`  
		Last Modified: Wed, 03 May 2023 04:32:31 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb4ecca0a280d864aad293e957efa59a8d6a2458bb34589a68df325ab9521e`  
		Last Modified: Wed, 03 May 2023 04:32:31 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2314ca77da3e599d8ca7b1fdd11a671f6ac79aaa627565d8252d55b02682a5`  
		Last Modified: Wed, 03 May 2023 04:32:56 GMT  
		Size: 216.5 MB (216487559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122debe1b6af34d1fba2a5f35e7e52b3c15ea04c754b7b2f39501489156158b7`  
		Last Modified: Wed, 03 May 2023 04:32:31 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:d0aa2588161968b9ed7b2d6e60a11fc0a7ce9c677fd1efd9cbb23d7aef163d74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.8 MB (247790020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02771e6e39ba06aab8020eab34a1b4de031cca6c42076545b26bc6ad3f81c92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:57:21 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 03 May 2023 03:47:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:47:47 GMT
ENV GOSU_VERSION=1.16
# Wed, 03 May 2023 03:47:47 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 03 May 2023 03:47:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 May 2023 03:47:55 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 May 2023 03:47:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 03 May 2023 03:47:57 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 03 May 2023 03:47:57 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 03 May 2023 03:47:57 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 03 May 2023 03:47:57 GMT
ENV MONGO_MAJOR=5.0
# Wed, 03 May 2023 03:47:57 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 03 May 2023 03:47:57 GMT
ENV MONGO_VERSION=5.0.17
# Wed, 03 May 2023 03:48:22 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 03 May 2023 03:48:25 GMT
VOLUME [/data/db /data/configdb]
# Wed, 03 May 2023 03:48:25 GMT
ENV HOME=/data/db
# Wed, 03 May 2023 03:48:25 GMT
COPY file:e3d6a34db83fe880626bff5d0b8d720ae43720caac9c739cbd1d336a129dad2d in /usr/local/bin/ 
# Wed, 03 May 2023 03:48:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:48:26 GMT
EXPOSE 27017
# Wed, 03 May 2023 03:48:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06c7ba53fe6d965200e96c72021fd3bee66138e7ae32fda40347d832ca07c4c`  
		Last Modified: Tue, 18 Apr 2023 01:59:09 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98de930ed0eb92a28b1702a22726d9e7e758797d1d25717a0cd817996e0dd58`  
		Last Modified: Wed, 03 May 2023 03:51:06 GMT  
		Size: 8.2 MB (8179716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3506d1a4618d9841c72c1c1cdcd5ee3a21454c69647995922f810059f9800d8d`  
		Last Modified: Wed, 03 May 2023 03:51:06 GMT  
		Size: 1.2 MB (1188964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471e077bfc9d9ff7b181540272893c7b7d31af0bc48f43d2b627ed965070a67`  
		Last Modified: Wed, 03 May 2023 03:51:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdd3cd5ed47a18f05126ced9b393833613cc1be8141a5e15d8aa97216496613`  
		Last Modified: Wed, 03 May 2023 03:51:04 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8401c90bd27cb43ca18013e5b2d14cc2268bf3037892c4586823b2ec397960`  
		Last Modified: Wed, 03 May 2023 03:51:03 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b96b87c93de38c4ac465fa99653e3600279d3b03edd9e0579ec6b3e1c817b0`  
		Last Modified: Wed, 03 May 2023 03:51:21 GMT  
		Size: 211.2 MB (211216231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3e11f381e8d962dd2f8e62f3b2f556760d7b5084fe0d402d23b221063c5dc2`  
		Last Modified: Wed, 03 May 2023 03:51:03 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
