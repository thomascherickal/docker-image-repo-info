## `mongo:4-focal`

```console
$ docker pull mongo@sha256:9bae20f7d39c9fcad741a84654a89c821dc84afc9599ad4707219f0a203eeecc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4-focal` - linux; amd64

```console
$ docker pull mongo@sha256:8f4f7785e5d79cd869e4d248e0aea4bda2076b375ab9f60763df79e0ccbc6465
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.0 MB (175999042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:282680a38569d16a6876299645eae6bfc25ef8e0d53bc9823b4da0d42cd16f9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:16:11 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 16 Jun 2023 03:16:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:16:25 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 03:16:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 16 Jun 2023 03:16:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 03:16:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 16 Jun 2023 03:17:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 03:17:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 16 Jun 2023 03:17:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 16 Jun 2023 03:17:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 16 Jun 2023 03:17:11 GMT
ENV MONGO_MAJOR=4.4
# Fri, 16 Jun 2023 03:17:11 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 16 Jun 2023 03:17:11 GMT
ENV MONGO_VERSION=4.4.22
# Fri, 16 Jun 2023 03:17:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 16 Jun 2023 03:17:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 16 Jun 2023 03:17:31 GMT
ENV HOME=/data/db
# Fri, 16 Jun 2023 03:17:31 GMT
COPY file:e3d6a34db83fe880626bff5d0b8d720ae43720caac9c739cbd1d336a129dad2d in /usr/local/bin/ 
# Fri, 16 Jun 2023 03:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:17:31 GMT
EXPOSE 27017
# Fri, 16 Jun 2023 03:17:31 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53df01b8802d8a11abf18e4918e1e78d7727be2bd8ff0c2a35168e7206ea7f22`  
		Last Modified: Fri, 16 Jun 2023 03:18:36 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8a86eac8b1590516abe17d55efae907f2a2c0d2989fad4ea7a660b6a7d28dc`  
		Last Modified: Fri, 16 Jun 2023 03:18:37 GMT  
		Size: 8.4 MB (8374115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322659b0c253d9be027554e499802a449daafb9dc3df73b463aeaf8d3874fe3c`  
		Last Modified: Fri, 16 Jun 2023 03:18:37 GMT  
		Size: 1.3 MB (1256053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5757a47256c59793bb3da27d3d2932103b03f576259bd24b6195b24dd22ef`  
		Last Modified: Fri, 16 Jun 2023 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4297db77d3de4728316707d3e28435bfee7e848d987b60a477a6d0520cb24e7`  
		Last Modified: Fri, 16 Jun 2023 03:19:11 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d8af276f8e7ee85dbc2d5d3b8e12ca4489921f9f9e83b8c3dea4f80587b040`  
		Last Modified: Fri, 16 Jun 2023 03:19:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4a26f395f636e66d2bef3688ebee16f1111b2c47a40cebec474d6d81103b3f`  
		Last Modified: Fri, 16 Jun 2023 03:19:26 GMT  
		Size: 137.8 MB (137779643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4daad771d55338eb27a4be681774c1ad67df67a2687bd1a8a4812d63c3c604`  
		Last Modified: Fri, 16 Jun 2023 03:19:11 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e898e577ee5fdddd2465bbe04610ef27a0bc38e2e34c1d3ca4a76331844adaf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.6 MB (171638210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2192db1c66466ace520063eba1366639f41a483e3b8d27b54f04fb411bf17da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:29:55 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 16 Jun 2023 03:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:05 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 03:30:05 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 16 Jun 2023 03:30:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 03:30:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 16 Jun 2023 03:30:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 03:30:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 16 Jun 2023 03:30:43 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 16 Jun 2023 03:30:43 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 16 Jun 2023 03:30:43 GMT
ENV MONGO_MAJOR=4.4
# Fri, 16 Jun 2023 03:30:44 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 16 Jun 2023 03:30:44 GMT
ENV MONGO_VERSION=4.4.22
# Fri, 16 Jun 2023 03:30:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 16 Jun 2023 03:31:00 GMT
VOLUME [/data/db /data/configdb]
# Fri, 16 Jun 2023 03:31:00 GMT
ENV HOME=/data/db
# Fri, 16 Jun 2023 03:31:00 GMT
COPY file:e3d6a34db83fe880626bff5d0b8d720ae43720caac9c739cbd1d336a129dad2d in /usr/local/bin/ 
# Fri, 16 Jun 2023 03:31:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:00 GMT
EXPOSE 27017
# Fri, 16 Jun 2023 03:31:00 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfc7c1c337b98b8be801b579852e1a98fbf1462d2094e94bc91bc71568086b4`  
		Last Modified: Fri, 16 Jun 2023 03:31:54 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf22f4a6aeb3175130d837759f77c51d229c2a4c67ed0e28fba67be21ea5453`  
		Last Modified: Fri, 16 Jun 2023 03:31:55 GMT  
		Size: 8.2 MB (8203100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5119931e25244a8e7477adf5a7b92c0961f3680ce13858065279be0239cdc1ec`  
		Last Modified: Fri, 16 Jun 2023 03:31:54 GMT  
		Size: 1.2 MB (1189817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e68af3af74497c0f23b84a74132c52fb214dd35f78931db3af00726c42cc00`  
		Last Modified: Fri, 16 Jun 2023 03:31:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200bd5fa646fe2f53f5bffa4d60611544ec5300713dab33f5cefaac41905399f`  
		Last Modified: Fri, 16 Jun 2023 03:32:20 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f22cad5f930ec07dd2b00466566f782ff1171b240c85a438bbbe1cc0433fc2`  
		Last Modified: Fri, 16 Jun 2023 03:32:20 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918654ea624c31a4b9cabf361df0865d6e1742fbff48b8132945f8f3881e6e39`  
		Last Modified: Fri, 16 Jun 2023 03:32:32 GMT  
		Size: 135.0 MB (135036141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c9802af9a500277f6e5029cf4c782bd2e5c5d0f3761d5fb5448d4ddaa326f1`  
		Last Modified: Fri, 16 Jun 2023 03:32:20 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
