## `mongo:focal`

```console
$ docker pull mongo@sha256:813b2b5e7c589cb04d014dc6bea46f8c25727ddfa00402b1fc38ba09dd0600a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:focal` - linux; amd64

```console
$ docker pull mongo@sha256:162aaa6fc63f0df68c3ec5b851e2f3df730911523f0e72c04db6538c80a39311
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.4 MB (231360077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34d21a9eb5bcd6d6e270ee52153cb7503c6e3262f6f1ee652d3a6000867a6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:52:11 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 02 Sep 2022 03:52:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:52:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 02 Sep 2022 03:52:20 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 02 Sep 2022 03:52:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:52:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:52:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '39BD841E4BE5FB195A65400E6A26B1AE64C3C388'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Fri, 02 Sep 2022 03:52:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 02 Sep 2022 03:52:33 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 02 Sep 2022 03:52:33 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 02 Sep 2022 03:52:33 GMT
ENV MONGO_MAJOR=6.0
# Fri, 02 Sep 2022 03:52:34 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 02 Sep 2022 03:52:34 GMT
ENV MONGO_VERSION=6.0.1
# Fri, 02 Sep 2022 03:53:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 02 Sep 2022 03:53:01 GMT
VOLUME [/data/db /data/configdb]
# Fri, 02 Sep 2022 03:53:02 GMT
ENV HOME=/data/db
# Fri, 02 Sep 2022 03:53:02 GMT
COPY file:a062061dd38363517a589afdd763f61500b162faee89d415017c58fd70abe392 in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:53:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:53:02 GMT
EXPOSE 27017
# Fri, 02 Sep 2022 03:53:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9c8c301e0f21d7d0b229b7ce3bf5f73a8032a77f1fd0ead5a40ae2904e7386`  
		Last Modified: Fri, 02 Sep 2022 03:57:03 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73738965c4ce390367a607807b960c2c4cd8aa410fc4b1bea6ce71263c6725a8`  
		Last Modified: Fri, 02 Sep 2022 03:57:04 GMT  
		Size: 3.1 MB (3059566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd6635b9ddf662b5aad927979bc18877d5e93da5b68d0257bf589086be3fc24`  
		Last Modified: Fri, 02 Sep 2022 03:57:04 GMT  
		Size: 6.5 MB (6506072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a471eaa4ad67f863744ea2570d2995126f69ac4a5156455603a9308c2c915e`  
		Last Modified: Fri, 02 Sep 2022 03:57:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf274af89b0a0884f7e076b77aa392912a4199a2dc008ddcfce30b3dc843df5`  
		Last Modified: Fri, 02 Sep 2022 03:57:01 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fc489f2a3bae9cf2166f37d4fe0c5fcbfb452e62be136900d6695577033d3e`  
		Last Modified: Fri, 02 Sep 2022 03:57:01 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eff8a505292a7d3ec899885b0d14700a4993bf2380609c49fea9becefa2560f`  
		Last Modified: Fri, 02 Sep 2022 03:57:28 GMT  
		Size: 193.2 MB (193213007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ef4431fce786940af0b92e361b8205a8b5978873659ce799ea1ccf218634e1`  
		Last Modified: Fri, 02 Sep 2022 03:57:01 GMT  
		Size: 5.1 KB (5071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b49cfcc3274a84d4b3f4c7574b8223253d6539285900fca7fed417c5e26bd945
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.6 MB (224590165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9db8e342ecea03db6856a2c4a7ab86235eae88a63a66bcf2a73e314fc905f3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:46:08 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 02 Aug 2022 18:46:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:46:42 GMT
ENV GOSU_VERSION=1.12
# Tue, 02 Aug 2022 18:46:43 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 02 Aug 2022 18:47:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 18:47:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 25 Aug 2022 00:05:57 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '39BD841E4BE5FB195A65400E6A26B1AE64C3C388'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Thu, 25 Aug 2022 00:05:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 25 Aug 2022 00:05:59 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 25 Aug 2022 00:06:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 25 Aug 2022 00:06:01 GMT
ENV MONGO_MAJOR=6.0
# Thu, 25 Aug 2022 00:06:02 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 25 Aug 2022 00:06:03 GMT
ENV MONGO_VERSION=6.0.1
# Thu, 25 Aug 2022 00:06:26 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 25 Aug 2022 00:06:27 GMT
VOLUME [/data/db /data/configdb]
# Thu, 25 Aug 2022 00:06:27 GMT
ENV HOME=/data/db
# Thu, 25 Aug 2022 19:05:31 GMT
COPY file:a062061dd38363517a589afdd763f61500b162faee89d415017c58fd70abe392 in /usr/local/bin/ 
# Thu, 25 Aug 2022 19:05:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 19:05:32 GMT
EXPOSE 27017
# Thu, 25 Aug 2022 19:05:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f92e7525120387a6bc9ec42b9ebfc8115309ab70f65a766e3fda1239d787f9`  
		Last Modified: Tue, 02 Aug 2022 18:51:20 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdda1347325980782ee9b7c6232d712c262b77bc097f712508cf17423dea0de`  
		Last Modified: Tue, 02 Aug 2022 18:51:21 GMT  
		Size: 2.9 MB (2907020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e02463a0f47d7c309281cbc5b4603815ec64c4653d4ed4ac37a06e6bb91b8e`  
		Last Modified: Tue, 02 Aug 2022 18:51:21 GMT  
		Size: 6.2 MB (6249317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9bc5b0968e9dc0079b9ed64930bcf14f8d69847b72f526a1dd1c8bd43df8cc`  
		Last Modified: Tue, 02 Aug 2022 18:51:18 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2908ff18ddc6a5d8953c967541541e6d401812961170bff48186d0847f9c13d3`  
		Last Modified: Thu, 25 Aug 2022 00:08:01 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966857d017e4236793227a8b33a78aab26fe08ce8ef7741e219ebe0854f4e70b`  
		Last Modified: Thu, 25 Aug 2022 00:08:01 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691117dd4546dbb52bbbbf3aa3bb25da617a11d6f5d26952e103b31232b8d7a1`  
		Last Modified: Thu, 25 Aug 2022 00:08:28 GMT  
		Size: 188.2 MB (188233402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d12f044cd7ff8e06e79e33df01201b4207ae04de1b5a371e4109987ff0a4f8`  
		Last Modified: Thu, 25 Aug 2022 19:07:07 GMT  
		Size: 5.1 KB (5072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
