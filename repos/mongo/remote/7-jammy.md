## `mongo:7-jammy`

```console
$ docker pull mongo@sha256:5b05f9d9ba230dc4afe31e9b3de4666a466c4fc8131aeefc03728221bd15c314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:7-jammy` - linux; amd64

```console
$ docker pull mongo@sha256:3ee80b67778b162efb3323c1f1539c573c9928c0540a567ebf5fec15d387327a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261144938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5acb2131d51f8ae39cbf4360b2f3f3e6d78dd14797bea477e173bb3c0e1abca7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:58:09 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 02 Dec 2023 04:58:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 04:58:18 GMT
ENV GOSU_VERSION=1.16
# Sat, 02 Dec 2023 04:58:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 02 Dec 2023 04:58:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 02 Dec 2023 04:58:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 02 Dec 2023 04:58:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'E58830201F7DD82CD808AA84160D26BB1785BA38'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 02 Dec 2023 04:58:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 02 Dec 2023 04:58:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 02 Dec 2023 04:58:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 02 Dec 2023 04:58:28 GMT
ENV MONGO_MAJOR=7.0
# Sat, 02 Dec 2023 04:58:28 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu jammy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 02 Dec 2023 04:58:28 GMT
ENV MONGO_VERSION=7.0.4
# Sat, 02 Dec 2023 04:58:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 		${MONGO_PACKAGE}-database=$MONGO_VERSION 		${MONGO_PACKAGE}-database-tools-extra=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 02 Dec 2023 04:58:54 GMT
VOLUME [/data/db /data/configdb]
# Sat, 02 Dec 2023 04:58:54 GMT
ENV HOME=/data/db
# Sat, 02 Dec 2023 04:58:54 GMT
COPY file:8fc8efb4e3db886ece2de8764459b4ab3e639e636ed08b2e828441229b4f8571 in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:58:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Dec 2023 04:58:55 GMT
EXPOSE 27017
# Sat, 02 Dec 2023 04:58:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80d99d2ce19b0e9c589171dbac0eac60bc4b3943817938ecfed3a8bd220d50b`  
		Last Modified: Sat, 02 Dec 2023 05:01:35 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb44dc221f386a8d7be81b66776b629685dd3cd74c5d31f00ef0357e74f09d2`  
		Last Modified: Sat, 02 Dec 2023 05:01:36 GMT  
		Size: 5.1 MB (5050736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52cece2eeeb646063bf149487118b7a1ea3ecf6c3f73c21c788fc4a7b1773494`  
		Last Modified: Sat, 02 Dec 2023 05:01:35 GMT  
		Size: 1.3 MB (1253151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9484737e86c40951589e2640a2f2210e5a7132e28618477889d94b5ebad6fa4d`  
		Last Modified: Sat, 02 Dec 2023 05:01:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ad935b75c0adbcb0eb26c035678f90309445dac9174d56c62b0847197ae180`  
		Last Modified: Sat, 02 Dec 2023 05:01:33 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ac6a8edff6b5e30bb7b32d2e4daaf7842dca49fd285553ce761bbdfba89220`  
		Last Modified: Sat, 02 Dec 2023 05:01:33 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90580617c703984ef681dfe4d159b7985600a8c042c8402ae3ce579ea47c3a80`  
		Last Modified: Sat, 02 Dec 2023 05:02:00 GMT  
		Size: 224.4 MB (224386050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c932f95934184a92c486807fcfe334b9b9a2bcdfdbd2ed4d42d2886e51d528c`  
		Last Modified: Sat, 02 Dec 2023 05:01:33 GMT  
		Size: 5.0 KB (5001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:7-jammy` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:9867cdf73ca72d3cea11907582d572ea8347cca929e1f988d7f784130bfe40b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.2 MB (253161028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df419f3480d4bb224ee76481332140203b909cc47f2319d796029df7f822625b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:08:19 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 02 Dec 2023 06:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:08:29 GMT
ENV GOSU_VERSION=1.16
# Sat, 02 Dec 2023 06:08:29 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 02 Dec 2023 06:08:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 02 Dec 2023 06:08:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 02 Dec 2023 06:08:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'E58830201F7DD82CD808AA84160D26BB1785BA38'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 02 Dec 2023 06:08:38 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 02 Dec 2023 06:08:38 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 02 Dec 2023 06:08:38 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 02 Dec 2023 06:08:38 GMT
ENV MONGO_MAJOR=7.0
# Sat, 02 Dec 2023 06:08:39 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu jammy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 02 Dec 2023 06:08:39 GMT
ENV MONGO_VERSION=7.0.4
# Sat, 02 Dec 2023 06:09:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 		${MONGO_PACKAGE}-database=$MONGO_VERSION 		${MONGO_PACKAGE}-database-tools-extra=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 02 Dec 2023 06:09:05 GMT
VOLUME [/data/db /data/configdb]
# Sat, 02 Dec 2023 06:09:05 GMT
ENV HOME=/data/db
# Sat, 02 Dec 2023 06:09:05 GMT
COPY file:8fc8efb4e3db886ece2de8764459b4ab3e639e636ed08b2e828441229b4f8571 in /usr/local/bin/ 
# Sat, 02 Dec 2023 06:09:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Dec 2023 06:09:05 GMT
EXPOSE 27017
# Sat, 02 Dec 2023 06:09:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855e7db284cb2e25fbca038c5f78c2f537b5f206a4190477bc774ad9f58c9a70`  
		Last Modified: Sat, 02 Dec 2023 06:11:25 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30996a99a88644ec076f14decff952d4850c7099203d0191615a0d66cd1133c2`  
		Last Modified: Sat, 02 Dec 2023 06:11:26 GMT  
		Size: 5.0 MB (4993914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1344348a6577e9231f9b1d5f3756b7ad0af9331fba6ea962fd881297fd5ef17`  
		Last Modified: Sat, 02 Dec 2023 06:11:25 GMT  
		Size: 1.2 MB (1186313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f396fecb61dcb05f6188ea3e29b0a5e283563de7650985f837cba2c889691175`  
		Last Modified: Sat, 02 Dec 2023 06:11:23 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297642578af2d3e2b9d17e57f36f6cd6ceec372a2c074fb0a3553a248ad23588`  
		Last Modified: Sat, 02 Dec 2023 06:11:23 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a06c0e8e6a354d917b2f4a2686f1836f056eb4fa3c0128289a03d650de10ef8`  
		Last Modified: Sat, 02 Dec 2023 06:11:23 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf265d6d56c3d20dbae06bcc074ce850324f3dc536fc5bc28b7948319d7f120b`  
		Last Modified: Sat, 02 Dec 2023 06:11:43 GMT  
		Size: 218.6 MB (218572188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d3269f1dc7ce2c6a9eeadd35208a702e7ab1343124d384564d48ea0a948eec`  
		Last Modified: Sat, 02 Dec 2023 06:11:23 GMT  
		Size: 5.0 KB (4998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
