## `mongo:5-focal`

```console
$ docker pull mongo@sha256:30bae100205286eb2489e82c5e13588c87587e7d31ad3eb3ccfd4f976910277c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:5-focal` - linux; amd64

```console
$ docker pull mongo@sha256:ec2874ea984979d2876b3ef8c361364245943440488ecc44b6e4dd81ae389a11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.4 MB (266356825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41b90b03613937ed61fe4b9f6f2347e431f836e3b22c4f41682ed5bd6b753c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 04:47:28 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 13 Oct 2023 04:47:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:47:50 GMT
ENV GOSU_VERSION=1.16
# Fri, 13 Oct 2023 04:47:50 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 13 Oct 2023 04:47:59 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 13 Oct 2023 04:47:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 13 Oct 2023 04:48:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 13 Oct 2023 04:48:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 13 Oct 2023 04:48:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 13 Oct 2023 04:48:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 13 Oct 2023 04:48:00 GMT
ENV MONGO_MAJOR=5.0
# Fri, 13 Oct 2023 04:48:01 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Oct 2023 23:20:40 GMT
ENV MONGO_VERSION=5.0.22
# Thu, 26 Oct 2023 23:21:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Oct 2023 23:21:18 GMT
VOLUME [/data/db /data/configdb]
# Thu, 26 Oct 2023 23:21:18 GMT
ENV HOME=/data/db
# Thu, 26 Oct 2023 23:21:18 GMT
COPY file:8fc8efb4e3db886ece2de8764459b4ab3e639e636ed08b2e828441229b4f8571 in /usr/local/bin/ 
# Thu, 26 Oct 2023 23:21:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 23:21:18 GMT
EXPOSE 27017
# Thu, 26 Oct 2023 23:21:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57cf58c4ffe57f0ecff1cc565b2fee1540eef321a7e9ac6a779b824603e3f5e`  
		Last Modified: Fri, 13 Oct 2023 04:50:59 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb145f2aa465bdd9b2bbb03f46c6ca49645ada631bc11ac9f8a1f6e839d9785`  
		Last Modified: Fri, 13 Oct 2023 04:51:01 GMT  
		Size: 8.4 MB (8374123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f83d52d64ecc161131500171c3bf58a64f365ec075dfe99e9afc57b212ba1f`  
		Last Modified: Fri, 13 Oct 2023 04:51:00 GMT  
		Size: 1.3 MB (1256079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e012812179b70496665c8de7ed887ac965d4fe5251a0f179a1b29688b8b5e0e`  
		Last Modified: Fri, 13 Oct 2023 04:50:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdf42961fe1a419fb32056b49c2946082b4d97f093c819c7cfa4f519778a43d`  
		Last Modified: Fri, 13 Oct 2023 04:50:57 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f501ea170131583c62e78a77be395ead038b7ce1553e997015fbfe3ce19579`  
		Last Modified: Fri, 13 Oct 2023 04:50:57 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0171c6553b9de2eda417012a2af4bbcf1f9d174c497f963ab5f9716bbc1dd106`  
		Last Modified: Thu, 26 Oct 2023 23:22:57 GMT  
		Size: 228.1 MB (228137257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e91849ea3d06c23702a3e55cc783309e807443785aae014da9a0f41bbdab90`  
		Last Modified: Thu, 26 Oct 2023 23:22:31 GMT  
		Size: 5.0 KB (4998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e1702be0b136ece5513cd3ba97f1a0f8020efed28b8765ff9348acc77f540395
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256321388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba66b284d41b02cff9bb2a424b2f420a260d8ac3be2ea76d005ae713fab574c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:09:24 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 13 Oct 2023 05:10:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 05:10:10 GMT
ENV GOSU_VERSION=1.16
# Fri, 13 Oct 2023 05:10:10 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 13 Oct 2023 05:10:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 13 Oct 2023 05:10:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 13 Oct 2023 05:10:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 13 Oct 2023 05:10:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 13 Oct 2023 05:10:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 13 Oct 2023 05:10:20 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 13 Oct 2023 05:10:20 GMT
ENV MONGO_MAJOR=5.0
# Fri, 13 Oct 2023 05:10:20 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 13 Oct 2023 05:10:20 GMT
ENV MONGO_VERSION=5.0.21
# Fri, 13 Oct 2023 05:10:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 13 Oct 2023 05:10:50 GMT
VOLUME [/data/db /data/configdb]
# Fri, 13 Oct 2023 05:10:50 GMT
ENV HOME=/data/db
# Fri, 13 Oct 2023 05:10:51 GMT
COPY file:8fc8efb4e3db886ece2de8764459b4ab3e639e636ed08b2e828441229b4f8571 in /usr/local/bin/ 
# Fri, 13 Oct 2023 05:10:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 05:10:51 GMT
EXPOSE 27017
# Fri, 13 Oct 2023 05:10:51 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b8a8f6982dd8543e2d7fd40d8f91e6309d0c05e390dc5b334b67e256b958a2`  
		Last Modified: Fri, 13 Oct 2023 05:12:47 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c200bca1fe77ec7f3d81e8184db84343b21a8f5a5716a114e8757630c419f57e`  
		Last Modified: Fri, 13 Oct 2023 05:12:48 GMT  
		Size: 8.2 MB (8202367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c526910ee08da1a854493892a8c43d4429cc1ea180ce68d3494469e45be7b8c4`  
		Last Modified: Fri, 13 Oct 2023 05:12:47 GMT  
		Size: 1.2 MB (1189124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa0323df32ebd9c85f7a9b4745468fdf035c319ce3a6cf5c26ff2a58764693a`  
		Last Modified: Fri, 13 Oct 2023 05:12:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a60706d3c7c4fd4432368201105fb51c1327eeceb40b79ab47ada97cef0184`  
		Last Modified: Fri, 13 Oct 2023 05:12:44 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730a4323d9a89d290e497140a9c999287677c447926a1a6b1c0cf13d6fed769`  
		Last Modified: Fri, 13 Oct 2023 05:12:45 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bfe7f73e31b2d961246952bc632c9e852c89d8a89c275d01d2bcdbaf408fe5`  
		Last Modified: Fri, 13 Oct 2023 05:13:04 GMT  
		Size: 219.7 MB (219721701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c7c7966c8c1e5b042184b6b2c636c796f9771730372bc981d4c5cc59ee19cc`  
		Last Modified: Fri, 13 Oct 2023 05:12:45 GMT  
		Size: 5.0 KB (5001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
