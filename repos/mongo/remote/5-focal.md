## `mongo:5-focal`

```console
$ docker pull mongo@sha256:b338de9faee1612edcb41ab542b113d8c7ad1119f1555ea5e8f9d051135f7981
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:5-focal` - linux; amd64

```console
$ docker pull mongo@sha256:115de155651619065c913f6f6c0384823fead4fc241f864ceec7bc13a2298295
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255345671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c054b5e8e78efcfee9f7c926ffe5cebaa80143b10cefb9c6312751d0a8e96c`
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
# Fri, 16 Jun 2023 03:16:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 03:16:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 16 Jun 2023 03:16:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 16 Jun 2023 03:16:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 16 Jun 2023 03:16:34 GMT
ENV MONGO_MAJOR=5.0
# Fri, 16 Jun 2023 03:16:35 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 16 Jun 2023 03:16:35 GMT
ENV MONGO_VERSION=5.0.18
# Fri, 16 Jun 2023 03:16:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 16 Jun 2023 03:16:59 GMT
VOLUME [/data/db /data/configdb]
# Fri, 16 Jun 2023 03:16:59 GMT
ENV HOME=/data/db
# Fri, 16 Jun 2023 03:16:59 GMT
COPY file:e3d6a34db83fe880626bff5d0b8d720ae43720caac9c739cbd1d336a129dad2d in /usr/local/bin/ 
# Fri, 16 Jun 2023 03:16:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:17:00 GMT
EXPOSE 27017
# Fri, 16 Jun 2023 03:17:00 GMT
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
	-	`sha256:5841b3116002ecd8823119f3f5d9b1c88e7beca62c8e0800c0c0a7d3858e1fc4`  
		Last Modified: Fri, 16 Jun 2023 03:18:34 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcadb60d7196b007d77f123c05371b0e2dcdf68fe68fe05e4bbd655856db419`  
		Last Modified: Fri, 16 Jun 2023 03:18:34 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e8c75df73355516f042f3049c2c07f4ee2e6bb1398abb9528b57b234c1c2f0`  
		Last Modified: Fri, 16 Jun 2023 03:18:59 GMT  
		Size: 217.1 MB (217126275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523512229971f3470787816d8de37ae0df2caf8d3d8ca9bade37c2d109bcd31f`  
		Last Modified: Fri, 16 Jun 2023 03:18:34 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c76a8c33d50c083ef006292ef91ae6760a4883b47cff33628217496b88bae72f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248460840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:549084dd18d62bd70a77a3de4943202cd380c212a357673f0655324ae40a1761`
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
# Fri, 16 Jun 2023 03:30:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 03:30:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 16 Jun 2023 03:30:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 16 Jun 2023 03:30:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 16 Jun 2023 03:30:12 GMT
ENV MONGO_MAJOR=5.0
# Fri, 16 Jun 2023 03:30:13 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 16 Jun 2023 03:30:13 GMT
ENV MONGO_VERSION=5.0.18
# Fri, 16 Jun 2023 03:30:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 16 Jun 2023 03:30:36 GMT
VOLUME [/data/db /data/configdb]
# Fri, 16 Jun 2023 03:30:36 GMT
ENV HOME=/data/db
# Fri, 16 Jun 2023 03:30:36 GMT
COPY file:e3d6a34db83fe880626bff5d0b8d720ae43720caac9c739cbd1d336a129dad2d in /usr/local/bin/ 
# Fri, 16 Jun 2023 03:30:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:30:37 GMT
EXPOSE 27017
# Fri, 16 Jun 2023 03:30:37 GMT
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
	-	`sha256:15e52d1efe909a350b14ce9b69d28ff430509c88c3f94cd0fdc844653d7700d8`  
		Last Modified: Fri, 16 Jun 2023 03:31:52 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6110d688160da1d4f0296c323f96824db55bd94be0d09ca52ee6c391f389ac3f`  
		Last Modified: Fri, 16 Jun 2023 03:31:52 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f0567d4541dabb0944c2ee497be0fb7703c1e893c16a8d5dae4ebc09b0ef77`  
		Last Modified: Fri, 16 Jun 2023 03:32:10 GMT  
		Size: 211.9 MB (211858772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511320f06e3f1fbc8205e53e1e2836158e498cd71fafbe2e9748da2c2e13d971`  
		Last Modified: Fri, 16 Jun 2023 03:31:52 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
