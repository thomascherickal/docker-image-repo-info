<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.18`](#mongo3618)
-	[`mongo:3.6.18-windowsservercore`](#mongo3618-windowsservercore)
-	[`mongo:3.6.18-windowsservercore-1809`](#mongo3618-windowsservercore-1809)
-	[`mongo:3.6.18-windowsservercore-ltsc2016`](#mongo3618-windowsservercore-ltsc2016)
-	[`mongo:3.6.18-xenial`](#mongo3618-xenial)
-	[`mongo:3.6-windowsservercore`](#mongo36-windowsservercore)
-	[`mongo:3.6-windowsservercore-1809`](#mongo36-windowsservercore-1809)
-	[`mongo:3.6-windowsservercore-ltsc2016`](#mongo36-windowsservercore-ltsc2016)
-	[`mongo:3.6-xenial`](#mongo36-xenial)
-	[`mongo:3-windowsservercore`](#mongo3-windowsservercore)
-	[`mongo:3-windowsservercore-1809`](#mongo3-windowsservercore-1809)
-	[`mongo:3-windowsservercore-ltsc2016`](#mongo3-windowsservercore-ltsc2016)
-	[`mongo:3-xenial`](#mongo3-xenial)
-	[`mongo:4`](#mongo4)
-	[`mongo:4.0`](#mongo40)
-	[`mongo:4.0.18`](#mongo4018)
-	[`mongo:4.0.18-windowsservercore`](#mongo4018-windowsservercore)
-	[`mongo:4.0.18-windowsservercore-1809`](#mongo4018-windowsservercore-1809)
-	[`mongo:4.0.18-windowsservercore-ltsc2016`](#mongo4018-windowsservercore-ltsc2016)
-	[`mongo:4.0.18-xenial`](#mongo4018-xenial)
-	[`mongo:4.0-windowsservercore`](#mongo40-windowsservercore)
-	[`mongo:4.0-windowsservercore-1809`](#mongo40-windowsservercore-1809)
-	[`mongo:4.0-windowsservercore-ltsc2016`](#mongo40-windowsservercore-ltsc2016)
-	[`mongo:4.0-xenial`](#mongo40-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2.6`](#mongo426)
-	[`mongo:4.2.6-bionic`](#mongo426-bionic)
-	[`mongo:4.2.6-windowsservercore`](#mongo426-windowsservercore)
-	[`mongo:4.2.6-windowsservercore-1809`](#mongo426-windowsservercore-1809)
-	[`mongo:4.2.6-windowsservercore-ltsc2016`](#mongo426-windowsservercore-ltsc2016)
-	[`mongo:4.2-bionic`](#mongo42-bionic)
-	[`mongo:4.2-windowsservercore`](#mongo42-windowsservercore)
-	[`mongo:4.2-windowsservercore-1809`](#mongo42-windowsservercore-1809)
-	[`mongo:4.2-windowsservercore-ltsc2016`](#mongo42-windowsservercore-ltsc2016)
-	[`mongo:4-bionic`](#mongo4-bionic)
-	[`mongo:4-windowsservercore`](#mongo4-windowsservercore)
-	[`mongo:4-windowsservercore-1809`](#mongo4-windowsservercore-1809)
-	[`mongo:4-windowsservercore-ltsc2016`](#mongo4-windowsservercore-ltsc2016)
-	[`mongo:bionic`](#mongobionic)
-	[`mongo:latest`](#mongolatest)
-	[`mongo:windowsservercore`](#mongowindowsservercore)
-	[`mongo:windowsservercore-1809`](#mongowindowsservercore-1809)
-	[`mongo:windowsservercore-ltsc2016`](#mongowindowsservercore-ltsc2016)

## `mongo:3`

```console
$ docker pull mongo@sha256:a1b8477842c4467cabd4f9d80b2334b49e29d0dec329d366c296e8d2cd813229
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:685aba1be7c90b6b431b0d4afb569b41e133771a91bbae0898fd69f02da86832
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165868990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95b2c69031b8f7eda2835ffb5037623ad35f8d4bfd5ba0a92741885113f9c07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:00 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 21:59:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:19:53 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:19:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:20:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:20:18 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:20:18 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:20:18 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:20:19 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:20:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0910d5ee82935ca0c4dd7bb1f01d2bdf89d2bdca5b4fd5e093b8ff47a170d5fc`  
		Last Modified: Fri, 24 Apr 2020 22:01:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0890f4d1c4192c03a3bfe405d061ed499f2bde5c34fbad309659f14b9e2cf2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76f45b5a1996fd5ba1728b366dded1357b869a25e5d328978671e9c4e3ba88f`  
		Last Modified: Wed, 29 Apr 2020 17:21:06 GMT  
		Size: 117.4 MB (117360475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02252b2b1d703c5bede825ff25d0eb485fe2065eb3f701ed7490dc69ab910fb5`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78a04c03604e5257c5283ce5ff5c0f7ada8ee8c9cfa89d365bfe209c45aeba2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7cbffdc515dde30993f4729bc28178a7793c37c7f6ec25cea09a586d90340dfe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155248541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904f60e23127ab5d787e360a03a732704ac00384c650cc39a6046d30f91fabeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:10 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 16:17:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:17:13 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:17:14 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:14 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:15 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:40:10 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:40:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:40:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:40:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:40:44 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:40:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:40:46 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:40:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2027de0f6b664ea891ed435841a0d444186df6e88b5b5f2946927698336d6`  
		Last Modified: Fri, 24 Apr 2020 16:20:33 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51838de4593a3cf57cc1bbf4401b1e3317053d5b71836242355484569d6c9766`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5960b53a2baae9777bf2a0a13529242873bbd574a8d6571d26db58eb57fe88a`  
		Last Modified: Wed, 29 Apr 2020 17:41:44 GMT  
		Size: 111.6 MB (111562471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ae22431403f2d02e736d73be023188361e4bb176b02e81db211cdf2a25e8cf`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97de399de3fd392c1ec058cb2675242579798827df631819da690c86b009568`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:a1b8477842c4467cabd4f9d80b2334b49e29d0dec329d366c296e8d2cd813229
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:685aba1be7c90b6b431b0d4afb569b41e133771a91bbae0898fd69f02da86832
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165868990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95b2c69031b8f7eda2835ffb5037623ad35f8d4bfd5ba0a92741885113f9c07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:00 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 21:59:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:19:53 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:19:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:20:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:20:18 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:20:18 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:20:18 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:20:19 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:20:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0910d5ee82935ca0c4dd7bb1f01d2bdf89d2bdca5b4fd5e093b8ff47a170d5fc`  
		Last Modified: Fri, 24 Apr 2020 22:01:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0890f4d1c4192c03a3bfe405d061ed499f2bde5c34fbad309659f14b9e2cf2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76f45b5a1996fd5ba1728b366dded1357b869a25e5d328978671e9c4e3ba88f`  
		Last Modified: Wed, 29 Apr 2020 17:21:06 GMT  
		Size: 117.4 MB (117360475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02252b2b1d703c5bede825ff25d0eb485fe2065eb3f701ed7490dc69ab910fb5`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78a04c03604e5257c5283ce5ff5c0f7ada8ee8c9cfa89d365bfe209c45aeba2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7cbffdc515dde30993f4729bc28178a7793c37c7f6ec25cea09a586d90340dfe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155248541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904f60e23127ab5d787e360a03a732704ac00384c650cc39a6046d30f91fabeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:10 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 16:17:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:17:13 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:17:14 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:14 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:15 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:40:10 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:40:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:40:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:40:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:40:44 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:40:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:40:46 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:40:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2027de0f6b664ea891ed435841a0d444186df6e88b5b5f2946927698336d6`  
		Last Modified: Fri, 24 Apr 2020 16:20:33 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51838de4593a3cf57cc1bbf4401b1e3317053d5b71836242355484569d6c9766`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5960b53a2baae9777bf2a0a13529242873bbd574a8d6571d26db58eb57fe88a`  
		Last Modified: Wed, 29 Apr 2020 17:41:44 GMT  
		Size: 111.6 MB (111562471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ae22431403f2d02e736d73be023188361e4bb176b02e81db211cdf2a25e8cf`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97de399de3fd392c1ec058cb2675242579798827df631819da690c86b009568`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18`

```console
$ docker pull mongo@sha256:a1b8477842c4467cabd4f9d80b2334b49e29d0dec329d366c296e8d2cd813229
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:3.6.18` - linux; amd64

```console
$ docker pull mongo@sha256:685aba1be7c90b6b431b0d4afb569b41e133771a91bbae0898fd69f02da86832
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165868990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95b2c69031b8f7eda2835ffb5037623ad35f8d4bfd5ba0a92741885113f9c07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:00 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 21:59:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:19:53 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:19:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:20:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:20:18 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:20:18 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:20:18 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:20:19 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:20:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0910d5ee82935ca0c4dd7bb1f01d2bdf89d2bdca5b4fd5e093b8ff47a170d5fc`  
		Last Modified: Fri, 24 Apr 2020 22:01:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0890f4d1c4192c03a3bfe405d061ed499f2bde5c34fbad309659f14b9e2cf2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76f45b5a1996fd5ba1728b366dded1357b869a25e5d328978671e9c4e3ba88f`  
		Last Modified: Wed, 29 Apr 2020 17:21:06 GMT  
		Size: 117.4 MB (117360475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02252b2b1d703c5bede825ff25d0eb485fe2065eb3f701ed7490dc69ab910fb5`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78a04c03604e5257c5283ce5ff5c0f7ada8ee8c9cfa89d365bfe209c45aeba2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7cbffdc515dde30993f4729bc28178a7793c37c7f6ec25cea09a586d90340dfe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155248541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904f60e23127ab5d787e360a03a732704ac00384c650cc39a6046d30f91fabeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:10 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 16:17:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:17:13 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:17:14 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:14 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:15 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:40:10 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:40:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:40:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:40:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:40:44 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:40:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:40:46 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:40:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2027de0f6b664ea891ed435841a0d444186df6e88b5b5f2946927698336d6`  
		Last Modified: Fri, 24 Apr 2020 16:20:33 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51838de4593a3cf57cc1bbf4401b1e3317053d5b71836242355484569d6c9766`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5960b53a2baae9777bf2a0a13529242873bbd574a8d6571d26db58eb57fe88a`  
		Last Modified: Wed, 29 Apr 2020 17:41:44 GMT  
		Size: 111.6 MB (111562471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ae22431403f2d02e736d73be023188361e4bb176b02e81db211cdf2a25e8cf`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97de399de3fd392c1ec058cb2675242579798827df631819da690c86b009568`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18-windowsservercore`

```console
$ docker pull mongo@sha256:e326c829988e094587e628175e8ccc8dca65145db6cd1d203efdd10a59952a6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:3.6.18-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18-windowsservercore-1809`

```console
$ docker pull mongo@sha256:52df15ea4aaced6a7035556bb02d6a827ea8be1314662727d6543f14345230a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:3.6.18-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:06b77b67cd90a2df18d51fb4e66b0ac8b8b044d1f6993bc2eac6efdaa80d8d37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:3.6.18-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18-xenial`

```console
$ docker pull mongo@sha256:ff9cf5671bed88b7b425f1dcc2d2209e917334cf6882fb138c9e4ee974a09762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.18-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:685aba1be7c90b6b431b0d4afb569b41e133771a91bbae0898fd69f02da86832
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165868990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95b2c69031b8f7eda2835ffb5037623ad35f8d4bfd5ba0a92741885113f9c07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:00 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 21:59:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:19:53 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:19:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:20:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:20:18 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:20:18 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:20:18 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:20:19 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:20:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0910d5ee82935ca0c4dd7bb1f01d2bdf89d2bdca5b4fd5e093b8ff47a170d5fc`  
		Last Modified: Fri, 24 Apr 2020 22:01:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0890f4d1c4192c03a3bfe405d061ed499f2bde5c34fbad309659f14b9e2cf2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76f45b5a1996fd5ba1728b366dded1357b869a25e5d328978671e9c4e3ba88f`  
		Last Modified: Wed, 29 Apr 2020 17:21:06 GMT  
		Size: 117.4 MB (117360475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02252b2b1d703c5bede825ff25d0eb485fe2065eb3f701ed7490dc69ab910fb5`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78a04c03604e5257c5283ce5ff5c0f7ada8ee8c9cfa89d365bfe209c45aeba2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7cbffdc515dde30993f4729bc28178a7793c37c7f6ec25cea09a586d90340dfe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155248541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904f60e23127ab5d787e360a03a732704ac00384c650cc39a6046d30f91fabeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:10 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 16:17:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:17:13 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:17:14 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:14 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:15 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:40:10 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:40:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:40:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:40:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:40:44 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:40:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:40:46 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:40:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2027de0f6b664ea891ed435841a0d444186df6e88b5b5f2946927698336d6`  
		Last Modified: Fri, 24 Apr 2020 16:20:33 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51838de4593a3cf57cc1bbf4401b1e3317053d5b71836242355484569d6c9766`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5960b53a2baae9777bf2a0a13529242873bbd574a8d6571d26db58eb57fe88a`  
		Last Modified: Wed, 29 Apr 2020 17:41:44 GMT  
		Size: 111.6 MB (111562471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ae22431403f2d02e736d73be023188361e4bb176b02e81db211cdf2a25e8cf`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97de399de3fd392c1ec058cb2675242579798827df631819da690c86b009568`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:e326c829988e094587e628175e8ccc8dca65145db6cd1d203efdd10a59952a6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:52df15ea4aaced6a7035556bb02d6a827ea8be1314662727d6543f14345230a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:06b77b67cd90a2df18d51fb4e66b0ac8b8b044d1f6993bc2eac6efdaa80d8d37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:ff9cf5671bed88b7b425f1dcc2d2209e917334cf6882fb138c9e4ee974a09762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:685aba1be7c90b6b431b0d4afb569b41e133771a91bbae0898fd69f02da86832
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165868990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95b2c69031b8f7eda2835ffb5037623ad35f8d4bfd5ba0a92741885113f9c07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:00 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 21:59:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:19:53 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:19:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:20:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:20:18 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:20:18 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:20:18 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:20:19 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:20:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0910d5ee82935ca0c4dd7bb1f01d2bdf89d2bdca5b4fd5e093b8ff47a170d5fc`  
		Last Modified: Fri, 24 Apr 2020 22:01:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0890f4d1c4192c03a3bfe405d061ed499f2bde5c34fbad309659f14b9e2cf2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76f45b5a1996fd5ba1728b366dded1357b869a25e5d328978671e9c4e3ba88f`  
		Last Modified: Wed, 29 Apr 2020 17:21:06 GMT  
		Size: 117.4 MB (117360475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02252b2b1d703c5bede825ff25d0eb485fe2065eb3f701ed7490dc69ab910fb5`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78a04c03604e5257c5283ce5ff5c0f7ada8ee8c9cfa89d365bfe209c45aeba2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7cbffdc515dde30993f4729bc28178a7793c37c7f6ec25cea09a586d90340dfe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155248541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904f60e23127ab5d787e360a03a732704ac00384c650cc39a6046d30f91fabeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:10 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 16:17:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:17:13 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:17:14 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:14 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:15 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:40:10 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:40:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:40:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:40:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:40:44 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:40:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:40:46 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:40:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2027de0f6b664ea891ed435841a0d444186df6e88b5b5f2946927698336d6`  
		Last Modified: Fri, 24 Apr 2020 16:20:33 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51838de4593a3cf57cc1bbf4401b1e3317053d5b71836242355484569d6c9766`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5960b53a2baae9777bf2a0a13529242873bbd574a8d6571d26db58eb57fe88a`  
		Last Modified: Wed, 29 Apr 2020 17:41:44 GMT  
		Size: 111.6 MB (111562471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ae22431403f2d02e736d73be023188361e4bb176b02e81db211cdf2a25e8cf`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97de399de3fd392c1ec058cb2675242579798827df631819da690c86b009568`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:e326c829988e094587e628175e8ccc8dca65145db6cd1d203efdd10a59952a6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:3-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:52df15ea4aaced6a7035556bb02d6a827ea8be1314662727d6543f14345230a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:0a44aa02f7ec1830a37201c6da51b4d7fa7ec350a1d3dba40b5507cbda7ef6d7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2169169404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9768d2ed6d89a4f0b69849a9738a3721d503118b042ef0de7cd396ec36170271`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:15:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 19:15:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 19:15:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:38:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:38:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:38:26 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:38:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d3fde31da60a18bbcf98b72cf22080821980deb899ccfb8bcc5678b2574631`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad9773c3a587f80bbcf79f041ade38a6494ff03e132ea714ac2ba513301fe8`  
		Last Modified: Wed, 13 May 2020 20:59:33 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d772b07be4e2c358d75115a98840da7ea90b03d9a19d6239bca14183417dbe`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6588f0935ee298110624495a0ca1e26ecec7db0b9763a3d0ac949d188efef3c1`  
		Last Modified: Wed, 13 May 2020 21:00:54 GMT  
		Size: 450.8 MB (450828531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b3d08198829e3856a8be7f9ed76cd0835f81ed4031c193613f431b6cefdcb`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6842a9dc534dcf322805adc02c920db80cb5bafd07a3bcd35fd787c98f8c6`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23527c617d055f2ce41eaec5d4138475093fa81278aa51e4c88056098125c285`  
		Last Modified: Wed, 13 May 2020 20:59:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:06b77b67cd90a2df18d51fb4e66b0ac8b8b044d1f6993bc2eac6efdaa80d8d37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:ff9cf5671bed88b7b425f1dcc2d2209e917334cf6882fb138c9e4ee974a09762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:685aba1be7c90b6b431b0d4afb569b41e133771a91bbae0898fd69f02da86832
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165868990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95b2c69031b8f7eda2835ffb5037623ad35f8d4bfd5ba0a92741885113f9c07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:00 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 21:59:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:02 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:19:53 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:19:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:20:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:20:18 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:20:18 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:20:18 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:20:19 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:20:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0910d5ee82935ca0c4dd7bb1f01d2bdf89d2bdca5b4fd5e093b8ff47a170d5fc`  
		Last Modified: Fri, 24 Apr 2020 22:01:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0890f4d1c4192c03a3bfe405d061ed499f2bde5c34fbad309659f14b9e2cf2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76f45b5a1996fd5ba1728b366dded1357b869a25e5d328978671e9c4e3ba88f`  
		Last Modified: Wed, 29 Apr 2020 17:21:06 GMT  
		Size: 117.4 MB (117360475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02252b2b1d703c5bede825ff25d0eb485fe2065eb3f701ed7490dc69ab910fb5`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78a04c03604e5257c5283ce5ff5c0f7ada8ee8c9cfa89d365bfe209c45aeba2`  
		Last Modified: Wed, 29 Apr 2020 17:20:41 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7cbffdc515dde30993f4729bc28178a7793c37c7f6ec25cea09a586d90340dfe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155248541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904f60e23127ab5d787e360a03a732704ac00384c650cc39a6046d30f91fabeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:10 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 24 Apr 2020 16:17:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:17:13 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:17:14 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:14 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:17:15 GMT
ENV MONGO_MAJOR=3.6
# Wed, 29 Apr 2020 17:40:10 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 29 Apr 2020 17:40:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 29 Apr 2020 17:40:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 29 Apr 2020 17:40:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 29 Apr 2020 17:40:44 GMT
VOLUME [/data/db /data/configdb]
# Wed, 29 Apr 2020 17:40:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 29 Apr 2020 17:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 17:40:46 GMT
EXPOSE 27017
# Wed, 29 Apr 2020 17:40:46 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2027de0f6b664ea891ed435841a0d444186df6e88b5b5f2946927698336d6`  
		Last Modified: Fri, 24 Apr 2020 16:20:33 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51838de4593a3cf57cc1bbf4401b1e3317053d5b71836242355484569d6c9766`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5960b53a2baae9777bf2a0a13529242873bbd574a8d6571d26db58eb57fe88a`  
		Last Modified: Wed, 29 Apr 2020 17:41:44 GMT  
		Size: 111.6 MB (111562471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ae22431403f2d02e736d73be023188361e4bb176b02e81db211cdf2a25e8cf`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97de399de3fd392c1ec058cb2675242579798827df631819da690c86b009568`  
		Last Modified: Wed, 29 Apr 2020 17:41:19 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:c880f6b56f443bb4d01baa759883228cd84fa8d78fa1a36001d1c0a0712b5a07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:8c48baa1571469d7f5ae6d603b92b8027ada5eb39826c009cb33a13b46864908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164649492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3daf8637573f4568ba35ee0f818aa25384f547b6e9cfa0c9bf39b92d5a63da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:59:56 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 22:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 22:00:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 22:00:13 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 22:00:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 22:00:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 22:00:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 22:00:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 22:00:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 22:00:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 22:00:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 22:00:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 22:00:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 22:00:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 22:00:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 22:00:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 22:00:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 22:00:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d269900d94133efa09999e6bd3a64fc1f1ae303aa6a6196b82e8b39582d8a9`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2526abb80afdbc05f3785f8463ca88c113aa9028af96d085ea269cf7e601eb`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 3.0 MB (2981995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eece1f39ec6168fc3e4aaf7860fbeeb79e098e0df5d69b98f3612e65c48735`  
		Last Modified: Fri, 24 Apr 2020 22:01:56 GMT  
		Size: 5.8 MB (5823765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ed78d3204b906dde21c66c4f1c1008483ddd7ebdc6b86ba4e8b41c320fd4f`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a878b8604aebf98b3bc70ccfddeb849aefb3af253a340406b874a1a7f4e6442`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde03a2883d0ac5b63b567bc10a14f01eac2b63396f6fdeff8caed2eb3d25df7`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe534daa349b7d8b4a3eee9920bfa77e5a067f6c8698d81419fde9bb1f06d4`  
		Last Modified: Fri, 24 Apr 2020 22:02:13 GMT  
		Size: 129.1 MB (129109796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f164ba21e17cf867efb556e534bfdaf30d58988e36de4424ccedc5842f259579`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494c387442cc32b84937ca989fb819fa005f0dec31a42f16ef3817c47232c7f`  
		Last Modified: Fri, 24 Apr 2020 22:01:53 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:25821e16c7c401986caa09fba3be08b103203a1599edaba8cd34366903b4b3e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154693716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9c0f139339bf92dbef6e630dca8acc4265b72752f7d7b37e16786ed8d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:18:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:19:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:19:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:19:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:19:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:19:33 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 16:19:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:19:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:19:37 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:37 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 16:19:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:20:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:20:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:20:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:20:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:20:11 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:20:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8d1af89634c78002ec70ef345dd88801eff1bbca938f85fc7472acf873b32`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03832d333b77fecdaaf76768c24a0c6797373a576bd7fb9abc41f3e3e5e2e4`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 2.7 MB (2675928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6736a2d19b775007ab26e1c72ee2e84911c375eec60ec697fe5e8deca69f`  
		Last Modified: Fri, 24 Apr 2020 16:21:44 GMT  
		Size: 5.3 MB (5345352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aac5b0c675d956885986db6ac84f954ff2f6a98df26a133ae89ae619cd5be`  
		Last Modified: Fri, 24 Apr 2020 16:21:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53bf51618735c85e240ace69cf43a38a4077593fb9b4633fc1d85d2e655016`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296ff1757ed119711f3cc049cb72f1f77178850e6ba2efc6cb0d1e9e1687bdf`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697b84404da018afccd718c3454ed04a6ee05110f0d573a5d73e25a5c5cd75c`  
		Last Modified: Fri, 24 Apr 2020 16:22:09 GMT  
		Size: 122.9 MB (122907968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458af224982cf3028e9a2a89e362caa3e795382c0448adc60b4ab96bedbcc1ef`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7506dcffce0af812ecd82776f582f438856fd75e7f948fa2a689a841eaf272e0`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:9a853858232155d691db93ab8ab614ad4636f9465aaab10dad522c6ffdbb6fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160626574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6080841c0f9e130ab30d755a2610d8101b8b45a55cfbce1852edce8e90e15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:34:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 07:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:34:51 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 07:34:51 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 07:35:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 07:35:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 07:35:03 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 07:35:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 07:35:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 07:35:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 07:35:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 07:35:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 07:35:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:35:39 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 07:35:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c464d6728e9ac439c8d2dc10a88d64a54c34ac50926c66cb7b6d12e37b15d6`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd364a38efacff4956ad8e4082d7fa9593aa0a036757fdfbe97487eb26ea2c9`  
		Last Modified: Fri, 24 Apr 2020 07:36:03 GMT  
		Size: 2.7 MB (2714610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e788a62ef53016c8add2417fa25e2141e1b7293acd648f26ed2ddffd54e605b`  
		Last Modified: Fri, 24 Apr 2020 07:36:02 GMT  
		Size: 5.7 MB (5744825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e103dac172d8152c577b2075cc90e6b674188775064cccfbbbc84d93979b3e56`  
		Last Modified: Fri, 24 Apr 2020 07:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fb52c1ef634a5a074adebdaa3f4fc95e636e570c5719c5d662babed85392e`  
		Last Modified: Fri, 24 Apr 2020 07:35:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f95c28bb62ddcdbb79cc6870d5cd9701c912a6307bde4c657e1d0c619430fab`  
		Last Modified: Fri, 24 Apr 2020 07:35:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cea8c1238e8ec47654f290d7a566d006d9302762e741316cd236b909d4577d`  
		Last Modified: Fri, 24 Apr 2020 07:36:18 GMT  
		Size: 126.8 MB (126756767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873535c8ae6f6827fe3d880ab25b1cc404dc3b74898d2ca9bff17136b83caba`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d64c0289b5d5c3ee9e04955ed738543e81fdae4e1a43328fd4d88be18d402b`  
		Last Modified: Fri, 24 Apr 2020 07:36:30 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:225810f30af04088daab3d6dc1f7811f090acdc86ad467b8aeb18d720f284637
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:10e0dc106ba87ac31095daf8f36777cb30439b819f9eeea526d28d5aef11fc71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153717066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78b4116161e41eccdd131e7d8de17fcb221a39e36a975211784dd3a7247bd109`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:26 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 24 Apr 2020 21:59:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:27 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:27 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:28 GMT
ENV MONGO_MAJOR=4.0
# Fri, 24 Apr 2020 21:59:28 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 24 Apr 2020 21:59:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 21:59:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 21:59:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 21:59:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 21:59:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 21:59:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 21:59:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 21:59:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee1a54d416a025682b9866dddb1e1753ac8e873aa7a216610aab6905ee28e1`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656aceafd7b5e01602496c9ca4e55e425bb8138f102a862ad833830327b5bfb0`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2abb3b91b37e782d0d4af1e23858d1d13986772e778144f087552d6c950119`  
		Last Modified: Fri, 24 Apr 2020 22:01:49 GMT  
		Size: 105.2 MB (105209121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a922c8a6198f43f9e23b9b0c3e4beb77a0b953f73bad8fe9abed435e242a443e`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce025523c4e84a60fc8ddc6249e82195c5a24ddf34ea705e827a832edafc1ac`  
		Last Modified: Fri, 24 Apr 2020 22:01:33 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:2f2453d105ecfe52f2978b8461d4a4a6a756a329eae7adf18f08e6a6fb294fdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143329420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f9f050c13891b73d379f80d79a2a59c001147bc100c01f46470510c75a191d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 24 Apr 2020 16:18:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:18:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:18:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:18:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:18:03 GMT
ENV MONGO_MAJOR=4.0
# Fri, 24 Apr 2020 16:18:04 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 24 Apr 2020 16:18:05 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:18:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:18:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:18:34 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:18:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:18:36 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:18:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9cfbc7523eafd818f49310c0660145f99ef417b5e33fc14dde1a4e9c691e89`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176c609d312b2670f8da9e72294f1c225dafe5c5bacf1d01b76370affcf3a0ad`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ebf85bcab66a237a422958c4176d323878d5a01f16373925994a14b03decbc`  
		Last Modified: Fri, 24 Apr 2020 16:21:34 GMT  
		Size: 99.6 MB (99643925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8e46255fbd40183c4b284dbe92b867b802541e61f0457464eb134faae1f4e8`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc8fcc8a0a1a416a06738f37c1af475d21581ce7f1d91a46f67b033ca21ea39`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:fd852297f0806faa11aa7ff9ed63b7ae07af8d8611fc370471224d038517ea81
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6180891864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ac03b78d3a678f4af6fc41c026ad2485779bf1ceda7f53ee3f3277c5fceeb1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:38:41 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:38:42 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:38:43 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 19:56:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:56:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:56:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:56:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5193c041167ce65eb1e135a19d56b87c6eb477df95b30908b379c1c4a97d91a`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fff0d731f7edc9d560b902a9564f97107992af22d31f93acc7ddd101f9310`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1547048dbc3a1e537804644097e7b1854dba0ec379b49efb4f76500ae2069bb9`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e95593d617b2dda42d7d14932fe6c75e7e58d5a6283344a70e76364d98e363`  
		Last Modified: Wed, 13 May 2020 21:09:42 GMT  
		Size: 449.0 MB (448993862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a850f869505f7ccc9a19ecf58fe4b02e0834ad7bd202aca3e49b9c45f7d0684`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc98339d70ce213b5f86b7979e200019fe70332b7dd809440ed0abb81250547`  
		Last Modified: Wed, 13 May 2020 21:01:11 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e67966c0698d7708493f9cf696e3c7c565b59530b04876c470eb31b39ee9f8`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:f11e9bb92492b252f010b62bb5ce096ce116ba39d8b34d7cef1927d85b3dd73f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2162114642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d99eca762b2ff55811abcb29fd68959a40c328ff26898373d43b0641494c3c8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:56:44 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:56:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:56:46 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 20:16:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:16:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:16:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:16:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a747df4e6d0efd4e09142e9359593124b0337666d814b66e120fe65e649b84`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b0d227fa142b343090d2ac35f63beed509d8e250c68e7aebc785edd307db6`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504e16f0479ce5903d2f29501bab183b0ba196513fe53957a813c64f374c49b`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad16ed00200ff7beac0ea9562347e5b6e222891cdfbee4985b75a7f2a093daa`  
		Last Modified: Wed, 13 May 2020 21:17:53 GMT  
		Size: 443.8 MB (443773767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad873f1a78c77fba56626855a3eafffd74ccf6a7237ab829b390da0a1bd08c9`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79359752c27922f36eb6aa1b0e24eb2b04b800982fa886060c09fa6675864039`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ca704d497fe68df5b8f66e0e5a3a7c4d93d520de85839bec1f7ef4abdb1e41`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18`

```console
$ docker pull mongo@sha256:225810f30af04088daab3d6dc1f7811f090acdc86ad467b8aeb18d720f284637
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.0.18` - linux; amd64

```console
$ docker pull mongo@sha256:10e0dc106ba87ac31095daf8f36777cb30439b819f9eeea526d28d5aef11fc71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153717066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78b4116161e41eccdd131e7d8de17fcb221a39e36a975211784dd3a7247bd109`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:26 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 24 Apr 2020 21:59:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:27 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:27 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:28 GMT
ENV MONGO_MAJOR=4.0
# Fri, 24 Apr 2020 21:59:28 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 24 Apr 2020 21:59:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 21:59:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 21:59:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 21:59:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 21:59:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 21:59:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 21:59:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 21:59:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee1a54d416a025682b9866dddb1e1753ac8e873aa7a216610aab6905ee28e1`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656aceafd7b5e01602496c9ca4e55e425bb8138f102a862ad833830327b5bfb0`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2abb3b91b37e782d0d4af1e23858d1d13986772e778144f087552d6c950119`  
		Last Modified: Fri, 24 Apr 2020 22:01:49 GMT  
		Size: 105.2 MB (105209121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a922c8a6198f43f9e23b9b0c3e4beb77a0b953f73bad8fe9abed435e242a443e`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce025523c4e84a60fc8ddc6249e82195c5a24ddf34ea705e827a832edafc1ac`  
		Last Modified: Fri, 24 Apr 2020 22:01:33 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:2f2453d105ecfe52f2978b8461d4a4a6a756a329eae7adf18f08e6a6fb294fdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143329420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f9f050c13891b73d379f80d79a2a59c001147bc100c01f46470510c75a191d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 24 Apr 2020 16:18:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:18:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:18:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:18:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:18:03 GMT
ENV MONGO_MAJOR=4.0
# Fri, 24 Apr 2020 16:18:04 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 24 Apr 2020 16:18:05 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:18:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:18:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:18:34 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:18:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:18:36 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:18:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9cfbc7523eafd818f49310c0660145f99ef417b5e33fc14dde1a4e9c691e89`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176c609d312b2670f8da9e72294f1c225dafe5c5bacf1d01b76370affcf3a0ad`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ebf85bcab66a237a422958c4176d323878d5a01f16373925994a14b03decbc`  
		Last Modified: Fri, 24 Apr 2020 16:21:34 GMT  
		Size: 99.6 MB (99643925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8e46255fbd40183c4b284dbe92b867b802541e61f0457464eb134faae1f4e8`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc8fcc8a0a1a416a06738f37c1af475d21581ce7f1d91a46f67b033ca21ea39`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:fd852297f0806faa11aa7ff9ed63b7ae07af8d8611fc370471224d038517ea81
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6180891864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ac03b78d3a678f4af6fc41c026ad2485779bf1ceda7f53ee3f3277c5fceeb1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:38:41 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:38:42 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:38:43 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 19:56:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:56:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:56:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:56:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5193c041167ce65eb1e135a19d56b87c6eb477df95b30908b379c1c4a97d91a`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fff0d731f7edc9d560b902a9564f97107992af22d31f93acc7ddd101f9310`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1547048dbc3a1e537804644097e7b1854dba0ec379b49efb4f76500ae2069bb9`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e95593d617b2dda42d7d14932fe6c75e7e58d5a6283344a70e76364d98e363`  
		Last Modified: Wed, 13 May 2020 21:09:42 GMT  
		Size: 449.0 MB (448993862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a850f869505f7ccc9a19ecf58fe4b02e0834ad7bd202aca3e49b9c45f7d0684`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc98339d70ce213b5f86b7979e200019fe70332b7dd809440ed0abb81250547`  
		Last Modified: Wed, 13 May 2020 21:01:11 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e67966c0698d7708493f9cf696e3c7c565b59530b04876c470eb31b39ee9f8`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:f11e9bb92492b252f010b62bb5ce096ce116ba39d8b34d7cef1927d85b3dd73f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2162114642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d99eca762b2ff55811abcb29fd68959a40c328ff26898373d43b0641494c3c8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:56:44 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:56:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:56:46 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 20:16:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:16:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:16:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:16:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a747df4e6d0efd4e09142e9359593124b0337666d814b66e120fe65e649b84`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b0d227fa142b343090d2ac35f63beed509d8e250c68e7aebc785edd307db6`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504e16f0479ce5903d2f29501bab183b0ba196513fe53957a813c64f374c49b`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad16ed00200ff7beac0ea9562347e5b6e222891cdfbee4985b75a7f2a093daa`  
		Last Modified: Wed, 13 May 2020 21:17:53 GMT  
		Size: 443.8 MB (443773767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad873f1a78c77fba56626855a3eafffd74ccf6a7237ab829b390da0a1bd08c9`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79359752c27922f36eb6aa1b0e24eb2b04b800982fa886060c09fa6675864039`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ca704d497fe68df5b8f66e0e5a3a7c4d93d520de85839bec1f7ef4abdb1e41`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18-windowsservercore`

```console
$ docker pull mongo@sha256:20381435ae4c81d51e9200610b48ae25854bfaf8741cb0bc510f172028e7d4a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.0.18-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:fd852297f0806faa11aa7ff9ed63b7ae07af8d8611fc370471224d038517ea81
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6180891864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ac03b78d3a678f4af6fc41c026ad2485779bf1ceda7f53ee3f3277c5fceeb1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:38:41 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:38:42 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:38:43 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 19:56:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:56:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:56:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:56:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5193c041167ce65eb1e135a19d56b87c6eb477df95b30908b379c1c4a97d91a`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fff0d731f7edc9d560b902a9564f97107992af22d31f93acc7ddd101f9310`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1547048dbc3a1e537804644097e7b1854dba0ec379b49efb4f76500ae2069bb9`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e95593d617b2dda42d7d14932fe6c75e7e58d5a6283344a70e76364d98e363`  
		Last Modified: Wed, 13 May 2020 21:09:42 GMT  
		Size: 449.0 MB (448993862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a850f869505f7ccc9a19ecf58fe4b02e0834ad7bd202aca3e49b9c45f7d0684`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc98339d70ce213b5f86b7979e200019fe70332b7dd809440ed0abb81250547`  
		Last Modified: Wed, 13 May 2020 21:01:11 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e67966c0698d7708493f9cf696e3c7c565b59530b04876c470eb31b39ee9f8`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:f11e9bb92492b252f010b62bb5ce096ce116ba39d8b34d7cef1927d85b3dd73f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2162114642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d99eca762b2ff55811abcb29fd68959a40c328ff26898373d43b0641494c3c8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:56:44 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:56:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:56:46 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 20:16:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:16:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:16:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:16:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a747df4e6d0efd4e09142e9359593124b0337666d814b66e120fe65e649b84`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b0d227fa142b343090d2ac35f63beed509d8e250c68e7aebc785edd307db6`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504e16f0479ce5903d2f29501bab183b0ba196513fe53957a813c64f374c49b`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad16ed00200ff7beac0ea9562347e5b6e222891cdfbee4985b75a7f2a093daa`  
		Last Modified: Wed, 13 May 2020 21:17:53 GMT  
		Size: 443.8 MB (443773767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad873f1a78c77fba56626855a3eafffd74ccf6a7237ab829b390da0a1bd08c9`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79359752c27922f36eb6aa1b0e24eb2b04b800982fa886060c09fa6675864039`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ca704d497fe68df5b8f66e0e5a3a7c4d93d520de85839bec1f7ef4abdb1e41`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18-windowsservercore-1809`

```console
$ docker pull mongo@sha256:6d92b9a50446dfc667dece6fd1adf8e7bdfb9171d33ffdfc98e56b1c8522d48d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.0.18-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:f11e9bb92492b252f010b62bb5ce096ce116ba39d8b34d7cef1927d85b3dd73f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2162114642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d99eca762b2ff55811abcb29fd68959a40c328ff26898373d43b0641494c3c8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:56:44 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:56:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:56:46 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 20:16:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:16:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:16:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:16:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a747df4e6d0efd4e09142e9359593124b0337666d814b66e120fe65e649b84`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b0d227fa142b343090d2ac35f63beed509d8e250c68e7aebc785edd307db6`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504e16f0479ce5903d2f29501bab183b0ba196513fe53957a813c64f374c49b`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad16ed00200ff7beac0ea9562347e5b6e222891cdfbee4985b75a7f2a093daa`  
		Last Modified: Wed, 13 May 2020 21:17:53 GMT  
		Size: 443.8 MB (443773767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad873f1a78c77fba56626855a3eafffd74ccf6a7237ab829b390da0a1bd08c9`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79359752c27922f36eb6aa1b0e24eb2b04b800982fa886060c09fa6675864039`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ca704d497fe68df5b8f66e0e5a3a7c4d93d520de85839bec1f7ef4abdb1e41`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:3e228e59b9c94c05376af2d6d20392bea1ad46dff106726f11ef593f565112e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4.0.18-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:fd852297f0806faa11aa7ff9ed63b7ae07af8d8611fc370471224d038517ea81
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6180891864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ac03b78d3a678f4af6fc41c026ad2485779bf1ceda7f53ee3f3277c5fceeb1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:38:41 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:38:42 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:38:43 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 19:56:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:56:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:56:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:56:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5193c041167ce65eb1e135a19d56b87c6eb477df95b30908b379c1c4a97d91a`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fff0d731f7edc9d560b902a9564f97107992af22d31f93acc7ddd101f9310`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1547048dbc3a1e537804644097e7b1854dba0ec379b49efb4f76500ae2069bb9`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e95593d617b2dda42d7d14932fe6c75e7e58d5a6283344a70e76364d98e363`  
		Last Modified: Wed, 13 May 2020 21:09:42 GMT  
		Size: 449.0 MB (448993862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a850f869505f7ccc9a19ecf58fe4b02e0834ad7bd202aca3e49b9c45f7d0684`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc98339d70ce213b5f86b7979e200019fe70332b7dd809440ed0abb81250547`  
		Last Modified: Wed, 13 May 2020 21:01:11 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e67966c0698d7708493f9cf696e3c7c565b59530b04876c470eb31b39ee9f8`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18-xenial`

```console
$ docker pull mongo@sha256:735463688aaeda0b61b74a76b4c951b34ce11b4ab247a7fa268fdec5bc155ac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.18-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:10e0dc106ba87ac31095daf8f36777cb30439b819f9eeea526d28d5aef11fc71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153717066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78b4116161e41eccdd131e7d8de17fcb221a39e36a975211784dd3a7247bd109`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:26 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 24 Apr 2020 21:59:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:27 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:27 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:28 GMT
ENV MONGO_MAJOR=4.0
# Fri, 24 Apr 2020 21:59:28 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 24 Apr 2020 21:59:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 21:59:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 21:59:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 21:59:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 21:59:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 21:59:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 21:59:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 21:59:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee1a54d416a025682b9866dddb1e1753ac8e873aa7a216610aab6905ee28e1`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656aceafd7b5e01602496c9ca4e55e425bb8138f102a862ad833830327b5bfb0`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2abb3b91b37e782d0d4af1e23858d1d13986772e778144f087552d6c950119`  
		Last Modified: Fri, 24 Apr 2020 22:01:49 GMT  
		Size: 105.2 MB (105209121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a922c8a6198f43f9e23b9b0c3e4beb77a0b953f73bad8fe9abed435e242a443e`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce025523c4e84a60fc8ddc6249e82195c5a24ddf34ea705e827a832edafc1ac`  
		Last Modified: Fri, 24 Apr 2020 22:01:33 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:2f2453d105ecfe52f2978b8461d4a4a6a756a329eae7adf18f08e6a6fb294fdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143329420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f9f050c13891b73d379f80d79a2a59c001147bc100c01f46470510c75a191d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 24 Apr 2020 16:18:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:18:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:18:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:18:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:18:03 GMT
ENV MONGO_MAJOR=4.0
# Fri, 24 Apr 2020 16:18:04 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 24 Apr 2020 16:18:05 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:18:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:18:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:18:34 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:18:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:18:36 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:18:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9cfbc7523eafd818f49310c0660145f99ef417b5e33fc14dde1a4e9c691e89`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176c609d312b2670f8da9e72294f1c225dafe5c5bacf1d01b76370affcf3a0ad`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ebf85bcab66a237a422958c4176d323878d5a01f16373925994a14b03decbc`  
		Last Modified: Fri, 24 Apr 2020 16:21:34 GMT  
		Size: 99.6 MB (99643925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8e46255fbd40183c4b284dbe92b867b802541e61f0457464eb134faae1f4e8`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc8fcc8a0a1a416a06738f37c1af475d21581ce7f1d91a46f67b033ca21ea39`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:20381435ae4c81d51e9200610b48ae25854bfaf8741cb0bc510f172028e7d4a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:fd852297f0806faa11aa7ff9ed63b7ae07af8d8611fc370471224d038517ea81
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6180891864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ac03b78d3a678f4af6fc41c026ad2485779bf1ceda7f53ee3f3277c5fceeb1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:38:41 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:38:42 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:38:43 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 19:56:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:56:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:56:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:56:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5193c041167ce65eb1e135a19d56b87c6eb477df95b30908b379c1c4a97d91a`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fff0d731f7edc9d560b902a9564f97107992af22d31f93acc7ddd101f9310`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1547048dbc3a1e537804644097e7b1854dba0ec379b49efb4f76500ae2069bb9`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e95593d617b2dda42d7d14932fe6c75e7e58d5a6283344a70e76364d98e363`  
		Last Modified: Wed, 13 May 2020 21:09:42 GMT  
		Size: 449.0 MB (448993862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a850f869505f7ccc9a19ecf58fe4b02e0834ad7bd202aca3e49b9c45f7d0684`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc98339d70ce213b5f86b7979e200019fe70332b7dd809440ed0abb81250547`  
		Last Modified: Wed, 13 May 2020 21:01:11 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e67966c0698d7708493f9cf696e3c7c565b59530b04876c470eb31b39ee9f8`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:f11e9bb92492b252f010b62bb5ce096ce116ba39d8b34d7cef1927d85b3dd73f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2162114642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d99eca762b2ff55811abcb29fd68959a40c328ff26898373d43b0641494c3c8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:56:44 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:56:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:56:46 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 20:16:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:16:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:16:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:16:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a747df4e6d0efd4e09142e9359593124b0337666d814b66e120fe65e649b84`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b0d227fa142b343090d2ac35f63beed509d8e250c68e7aebc785edd307db6`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504e16f0479ce5903d2f29501bab183b0ba196513fe53957a813c64f374c49b`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad16ed00200ff7beac0ea9562347e5b6e222891cdfbee4985b75a7f2a093daa`  
		Last Modified: Wed, 13 May 2020 21:17:53 GMT  
		Size: 443.8 MB (443773767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad873f1a78c77fba56626855a3eafffd74ccf6a7237ab829b390da0a1bd08c9`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79359752c27922f36eb6aa1b0e24eb2b04b800982fa886060c09fa6675864039`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ca704d497fe68df5b8f66e0e5a3a7c4d93d520de85839bec1f7ef4abdb1e41`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:6d92b9a50446dfc667dece6fd1adf8e7bdfb9171d33ffdfc98e56b1c8522d48d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:f11e9bb92492b252f010b62bb5ce096ce116ba39d8b34d7cef1927d85b3dd73f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2162114642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d99eca762b2ff55811abcb29fd68959a40c328ff26898373d43b0641494c3c8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:56:44 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:56:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:56:46 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 20:16:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:16:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:16:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:16:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a747df4e6d0efd4e09142e9359593124b0337666d814b66e120fe65e649b84`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b0d227fa142b343090d2ac35f63beed509d8e250c68e7aebc785edd307db6`  
		Last Modified: Wed, 13 May 2020 21:09:56 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504e16f0479ce5903d2f29501bab183b0ba196513fe53957a813c64f374c49b`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad16ed00200ff7beac0ea9562347e5b6e222891cdfbee4985b75a7f2a093daa`  
		Last Modified: Wed, 13 May 2020 21:17:53 GMT  
		Size: 443.8 MB (443773767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad873f1a78c77fba56626855a3eafffd74ccf6a7237ab829b390da0a1bd08c9`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79359752c27922f36eb6aa1b0e24eb2b04b800982fa886060c09fa6675864039`  
		Last Modified: Wed, 13 May 2020 21:09:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ca704d497fe68df5b8f66e0e5a3a7c4d93d520de85839bec1f7ef4abdb1e41`  
		Last Modified: Wed, 13 May 2020 21:09:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:3e228e59b9c94c05376af2d6d20392bea1ad46dff106726f11ef593f565112e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:fd852297f0806faa11aa7ff9ed63b7ae07af8d8611fc370471224d038517ea81
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6180891864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ac03b78d3a678f4af6fc41c026ad2485779bf1ceda7f53ee3f3277c5fceeb1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 19:38:41 GMT
ENV MONGO_VERSION=4.0.18
# Wed, 13 May 2020 19:38:42 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Wed, 13 May 2020 19:38:43 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Wed, 13 May 2020 19:56:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:56:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:56:36 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:56:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5193c041167ce65eb1e135a19d56b87c6eb477df95b30908b379c1c4a97d91a`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fff0d731f7edc9d560b902a9564f97107992af22d31f93acc7ddd101f9310`  
		Last Modified: Wed, 13 May 2020 21:01:13 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1547048dbc3a1e537804644097e7b1854dba0ec379b49efb4f76500ae2069bb9`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e95593d617b2dda42d7d14932fe6c75e7e58d5a6283344a70e76364d98e363`  
		Last Modified: Wed, 13 May 2020 21:09:42 GMT  
		Size: 449.0 MB (448993862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a850f869505f7ccc9a19ecf58fe4b02e0834ad7bd202aca3e49b9c45f7d0684`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc98339d70ce213b5f86b7979e200019fe70332b7dd809440ed0abb81250547`  
		Last Modified: Wed, 13 May 2020 21:01:11 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e67966c0698d7708493f9cf696e3c7c565b59530b04876c470eb31b39ee9f8`  
		Last Modified: Wed, 13 May 2020 21:01:10 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:735463688aaeda0b61b74a76b4c951b34ce11b4ab247a7fa268fdec5bc155ac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:10e0dc106ba87ac31095daf8f36777cb30439b819f9eeea526d28d5aef11fc71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153717066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78b4116161e41eccdd131e7d8de17fcb221a39e36a975211784dd3a7247bd109`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:58:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 21:58:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 21:58:48 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 21:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 21:59:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 21:59:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 21:59:26 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 24 Apr 2020 21:59:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 21:59:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 21:59:27 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:27 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 21:59:28 GMT
ENV MONGO_MAJOR=4.0
# Fri, 24 Apr 2020 21:59:28 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 24 Apr 2020 21:59:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 21:59:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 21:59:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 21:59:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 21:59:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 21:59:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 21:59:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 21:59:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef060c38165fe8e3bbd64fa5d00a9b1048a5f26720f798520783676e6da549f`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3640a82a5d85e12c636ee0b293ff9a4c0291adb4adb1b7b8fea5ddd7e21cab7`  
		Last Modified: Fri, 24 Apr 2020 22:01:08 GMT  
		Size: 2.9 MB (2946122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7a110209be387d3a81e03bc924c9e46c91541946ca9e7092ec9881847eb348`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 1.3 MB (1305289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6711959a41df17809aefa497b493d4092d7552afc3cb06ca2041293cd672871`  
		Last Modified: Fri, 24 Apr 2020 22:01:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee1a54d416a025682b9866dddb1e1753ac8e873aa7a216610aab6905ee28e1`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656aceafd7b5e01602496c9ca4e55e425bb8138f102a862ad833830327b5bfb0`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2abb3b91b37e782d0d4af1e23858d1d13986772e778144f087552d6c950119`  
		Last Modified: Fri, 24 Apr 2020 22:01:49 GMT  
		Size: 105.2 MB (105209121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a922c8a6198f43f9e23b9b0c3e4beb77a0b953f73bad8fe9abed435e242a443e`  
		Last Modified: Fri, 24 Apr 2020 22:01:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce025523c4e84a60fc8ddc6249e82195c5a24ddf34ea705e827a832edafc1ac`  
		Last Modified: Fri, 24 Apr 2020 22:01:33 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:2f2453d105ecfe52f2978b8461d4a4a6a756a329eae7adf18f08e6a6fb294fdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143329420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f9f050c13891b73d379f80d79a2a59c001147bc100c01f46470510c75a191d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:16:27 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:16:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:16:43 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:17:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:17:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:17:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 24 Apr 2020 16:18:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:18:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:18:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:18:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:18:03 GMT
ENV MONGO_MAJOR=4.0
# Fri, 24 Apr 2020 16:18:04 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 24 Apr 2020 16:18:05 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:18:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:18:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:18:34 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:18:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:18:36 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:18:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8e99e85782df175a29b1bde536a79db756966637facaf915cc8e16f38691`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d993ee733e416b83e56bc49a2736148b105b73cc7553c80fc2aaa7df313b1`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 2.5 MB (2475001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b49e909411104c2ebb353f5cd8c52434864e5d144971b58f81c3780a4cd037`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 1.2 MB (1232274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9944fff526a6c05418546fe52dfcdcf7b391b22af046c09426b603f2e7154`  
		Last Modified: Fri, 24 Apr 2020 16:20:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9cfbc7523eafd818f49310c0660145f99ef417b5e33fc14dde1a4e9c691e89`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176c609d312b2670f8da9e72294f1c225dafe5c5bacf1d01b76370affcf3a0ad`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ebf85bcab66a237a422958c4176d323878d5a01f16373925994a14b03decbc`  
		Last Modified: Fri, 24 Apr 2020 16:21:34 GMT  
		Size: 99.6 MB (99643925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8e46255fbd40183c4b284dbe92b867b802541e61f0457464eb134faae1f4e8`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc8fcc8a0a1a416a06738f37c1af475d21581ce7f1d91a46f67b033ca21ea39`  
		Last Modified: Fri, 24 Apr 2020 16:21:09 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:c880f6b56f443bb4d01baa759883228cd84fa8d78fa1a36001d1c0a0712b5a07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:8c48baa1571469d7f5ae6d603b92b8027ada5eb39826c009cb33a13b46864908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164649492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3daf8637573f4568ba35ee0f818aa25384f547b6e9cfa0c9bf39b92d5a63da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:59:56 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 22:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 22:00:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 22:00:13 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 22:00:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 22:00:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 22:00:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 22:00:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 22:00:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 22:00:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 22:00:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 22:00:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 22:00:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 22:00:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 22:00:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 22:00:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 22:00:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 22:00:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d269900d94133efa09999e6bd3a64fc1f1ae303aa6a6196b82e8b39582d8a9`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2526abb80afdbc05f3785f8463ca88c113aa9028af96d085ea269cf7e601eb`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 3.0 MB (2981995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eece1f39ec6168fc3e4aaf7860fbeeb79e098e0df5d69b98f3612e65c48735`  
		Last Modified: Fri, 24 Apr 2020 22:01:56 GMT  
		Size: 5.8 MB (5823765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ed78d3204b906dde21c66c4f1c1008483ddd7ebdc6b86ba4e8b41c320fd4f`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a878b8604aebf98b3bc70ccfddeb849aefb3af253a340406b874a1a7f4e6442`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde03a2883d0ac5b63b567bc10a14f01eac2b63396f6fdeff8caed2eb3d25df7`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe534daa349b7d8b4a3eee9920bfa77e5a067f6c8698d81419fde9bb1f06d4`  
		Last Modified: Fri, 24 Apr 2020 22:02:13 GMT  
		Size: 129.1 MB (129109796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f164ba21e17cf867efb556e534bfdaf30d58988e36de4424ccedc5842f259579`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494c387442cc32b84937ca989fb819fa005f0dec31a42f16ef3817c47232c7f`  
		Last Modified: Fri, 24 Apr 2020 22:01:53 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:25821e16c7c401986caa09fba3be08b103203a1599edaba8cd34366903b4b3e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154693716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9c0f139339bf92dbef6e630dca8acc4265b72752f7d7b37e16786ed8d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:18:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:19:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:19:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:19:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:19:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:19:33 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 16:19:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:19:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:19:37 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:37 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 16:19:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:20:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:20:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:20:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:20:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:20:11 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:20:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8d1af89634c78002ec70ef345dd88801eff1bbca938f85fc7472acf873b32`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03832d333b77fecdaaf76768c24a0c6797373a576bd7fb9abc41f3e3e5e2e4`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 2.7 MB (2675928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6736a2d19b775007ab26e1c72ee2e84911c375eec60ec697fe5e8deca69f`  
		Last Modified: Fri, 24 Apr 2020 16:21:44 GMT  
		Size: 5.3 MB (5345352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aac5b0c675d956885986db6ac84f954ff2f6a98df26a133ae89ae619cd5be`  
		Last Modified: Fri, 24 Apr 2020 16:21:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53bf51618735c85e240ace69cf43a38a4077593fb9b4633fc1d85d2e655016`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296ff1757ed119711f3cc049cb72f1f77178850e6ba2efc6cb0d1e9e1687bdf`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697b84404da018afccd718c3454ed04a6ee05110f0d573a5d73e25a5c5cd75c`  
		Last Modified: Fri, 24 Apr 2020 16:22:09 GMT  
		Size: 122.9 MB (122907968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458af224982cf3028e9a2a89e362caa3e795382c0448adc60b4ab96bedbcc1ef`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7506dcffce0af812ecd82776f582f438856fd75e7f948fa2a689a841eaf272e0`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; s390x

```console
$ docker pull mongo@sha256:9a853858232155d691db93ab8ab614ad4636f9465aaab10dad522c6ffdbb6fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160626574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6080841c0f9e130ab30d755a2610d8101b8b45a55cfbce1852edce8e90e15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:34:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 07:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:34:51 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 07:34:51 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 07:35:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 07:35:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 07:35:03 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 07:35:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 07:35:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 07:35:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 07:35:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 07:35:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 07:35:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:35:39 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 07:35:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c464d6728e9ac439c8d2dc10a88d64a54c34ac50926c66cb7b6d12e37b15d6`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd364a38efacff4956ad8e4082d7fa9593aa0a036757fdfbe97487eb26ea2c9`  
		Last Modified: Fri, 24 Apr 2020 07:36:03 GMT  
		Size: 2.7 MB (2714610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e788a62ef53016c8add2417fa25e2141e1b7293acd648f26ed2ddffd54e605b`  
		Last Modified: Fri, 24 Apr 2020 07:36:02 GMT  
		Size: 5.7 MB (5744825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e103dac172d8152c577b2075cc90e6b674188775064cccfbbbc84d93979b3e56`  
		Last Modified: Fri, 24 Apr 2020 07:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fb52c1ef634a5a074adebdaa3f4fc95e636e570c5719c5d662babed85392e`  
		Last Modified: Fri, 24 Apr 2020 07:35:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f95c28bb62ddcdbb79cc6870d5cd9701c912a6307bde4c657e1d0c619430fab`  
		Last Modified: Fri, 24 Apr 2020 07:35:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cea8c1238e8ec47654f290d7a566d006d9302762e741316cd236b909d4577d`  
		Last Modified: Fri, 24 Apr 2020 07:36:18 GMT  
		Size: 126.8 MB (126756767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873535c8ae6f6827fe3d880ab25b1cc404dc3b74898d2ca9bff17136b83caba`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d64c0289b5d5c3ee9e04955ed738543e81fdae4e1a43328fd4d88be18d402b`  
		Last Modified: Fri, 24 Apr 2020 07:36:30 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.6`

```console
$ docker pull mongo@sha256:c880f6b56f443bb4d01baa759883228cd84fa8d78fa1a36001d1c0a0712b5a07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2.6` - linux; amd64

```console
$ docker pull mongo@sha256:8c48baa1571469d7f5ae6d603b92b8027ada5eb39826c009cb33a13b46864908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164649492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3daf8637573f4568ba35ee0f818aa25384f547b6e9cfa0c9bf39b92d5a63da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:59:56 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 22:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 22:00:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 22:00:13 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 22:00:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 22:00:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 22:00:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 22:00:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 22:00:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 22:00:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 22:00:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 22:00:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 22:00:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 22:00:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 22:00:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 22:00:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 22:00:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 22:00:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d269900d94133efa09999e6bd3a64fc1f1ae303aa6a6196b82e8b39582d8a9`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2526abb80afdbc05f3785f8463ca88c113aa9028af96d085ea269cf7e601eb`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 3.0 MB (2981995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eece1f39ec6168fc3e4aaf7860fbeeb79e098e0df5d69b98f3612e65c48735`  
		Last Modified: Fri, 24 Apr 2020 22:01:56 GMT  
		Size: 5.8 MB (5823765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ed78d3204b906dde21c66c4f1c1008483ddd7ebdc6b86ba4e8b41c320fd4f`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a878b8604aebf98b3bc70ccfddeb849aefb3af253a340406b874a1a7f4e6442`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde03a2883d0ac5b63b567bc10a14f01eac2b63396f6fdeff8caed2eb3d25df7`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe534daa349b7d8b4a3eee9920bfa77e5a067f6c8698d81419fde9bb1f06d4`  
		Last Modified: Fri, 24 Apr 2020 22:02:13 GMT  
		Size: 129.1 MB (129109796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f164ba21e17cf867efb556e534bfdaf30d58988e36de4424ccedc5842f259579`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494c387442cc32b84937ca989fb819fa005f0dec31a42f16ef3817c47232c7f`  
		Last Modified: Fri, 24 Apr 2020 22:01:53 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:25821e16c7c401986caa09fba3be08b103203a1599edaba8cd34366903b4b3e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154693716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9c0f139339bf92dbef6e630dca8acc4265b72752f7d7b37e16786ed8d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:18:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:19:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:19:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:19:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:19:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:19:33 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 16:19:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:19:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:19:37 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:37 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 16:19:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:20:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:20:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:20:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:20:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:20:11 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:20:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8d1af89634c78002ec70ef345dd88801eff1bbca938f85fc7472acf873b32`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03832d333b77fecdaaf76768c24a0c6797373a576bd7fb9abc41f3e3e5e2e4`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 2.7 MB (2675928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6736a2d19b775007ab26e1c72ee2e84911c375eec60ec697fe5e8deca69f`  
		Last Modified: Fri, 24 Apr 2020 16:21:44 GMT  
		Size: 5.3 MB (5345352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aac5b0c675d956885986db6ac84f954ff2f6a98df26a133ae89ae619cd5be`  
		Last Modified: Fri, 24 Apr 2020 16:21:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53bf51618735c85e240ace69cf43a38a4077593fb9b4633fc1d85d2e655016`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296ff1757ed119711f3cc049cb72f1f77178850e6ba2efc6cb0d1e9e1687bdf`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697b84404da018afccd718c3454ed04a6ee05110f0d573a5d73e25a5c5cd75c`  
		Last Modified: Fri, 24 Apr 2020 16:22:09 GMT  
		Size: 122.9 MB (122907968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458af224982cf3028e9a2a89e362caa3e795382c0448adc60b4ab96bedbcc1ef`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7506dcffce0af812ecd82776f582f438856fd75e7f948fa2a689a841eaf272e0`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.6` - linux; s390x

```console
$ docker pull mongo@sha256:9a853858232155d691db93ab8ab614ad4636f9465aaab10dad522c6ffdbb6fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160626574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6080841c0f9e130ab30d755a2610d8101b8b45a55cfbce1852edce8e90e15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:34:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 07:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:34:51 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 07:34:51 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 07:35:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 07:35:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 07:35:03 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 07:35:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 07:35:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 07:35:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 07:35:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 07:35:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 07:35:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:35:39 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 07:35:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c464d6728e9ac439c8d2dc10a88d64a54c34ac50926c66cb7b6d12e37b15d6`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd364a38efacff4956ad8e4082d7fa9593aa0a036757fdfbe97487eb26ea2c9`  
		Last Modified: Fri, 24 Apr 2020 07:36:03 GMT  
		Size: 2.7 MB (2714610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e788a62ef53016c8add2417fa25e2141e1b7293acd648f26ed2ddffd54e605b`  
		Last Modified: Fri, 24 Apr 2020 07:36:02 GMT  
		Size: 5.7 MB (5744825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e103dac172d8152c577b2075cc90e6b674188775064cccfbbbc84d93979b3e56`  
		Last Modified: Fri, 24 Apr 2020 07:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fb52c1ef634a5a074adebdaa3f4fc95e636e570c5719c5d662babed85392e`  
		Last Modified: Fri, 24 Apr 2020 07:35:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f95c28bb62ddcdbb79cc6870d5cd9701c912a6307bde4c657e1d0c619430fab`  
		Last Modified: Fri, 24 Apr 2020 07:35:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cea8c1238e8ec47654f290d7a566d006d9302762e741316cd236b909d4577d`  
		Last Modified: Fri, 24 Apr 2020 07:36:18 GMT  
		Size: 126.8 MB (126756767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873535c8ae6f6827fe3d880ab25b1cc404dc3b74898d2ca9bff17136b83caba`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d64c0289b5d5c3ee9e04955ed738543e81fdae4e1a43328fd4d88be18d402b`  
		Last Modified: Fri, 24 Apr 2020 07:36:30 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.6` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.6` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.6-bionic`

```console
$ docker pull mongo@sha256:a89b09e8bc3153c5c87c52e36a7b6f992ee874c5329cc631e5d9542bf1cbfe31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2.6-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:8c48baa1571469d7f5ae6d603b92b8027ada5eb39826c009cb33a13b46864908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164649492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3daf8637573f4568ba35ee0f818aa25384f547b6e9cfa0c9bf39b92d5a63da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:59:56 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 22:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 22:00:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 22:00:13 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 22:00:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 22:00:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 22:00:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 22:00:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 22:00:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 22:00:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 22:00:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 22:00:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 22:00:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 22:00:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 22:00:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 22:00:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 22:00:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 22:00:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d269900d94133efa09999e6bd3a64fc1f1ae303aa6a6196b82e8b39582d8a9`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2526abb80afdbc05f3785f8463ca88c113aa9028af96d085ea269cf7e601eb`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 3.0 MB (2981995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eece1f39ec6168fc3e4aaf7860fbeeb79e098e0df5d69b98f3612e65c48735`  
		Last Modified: Fri, 24 Apr 2020 22:01:56 GMT  
		Size: 5.8 MB (5823765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ed78d3204b906dde21c66c4f1c1008483ddd7ebdc6b86ba4e8b41c320fd4f`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a878b8604aebf98b3bc70ccfddeb849aefb3af253a340406b874a1a7f4e6442`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde03a2883d0ac5b63b567bc10a14f01eac2b63396f6fdeff8caed2eb3d25df7`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe534daa349b7d8b4a3eee9920bfa77e5a067f6c8698d81419fde9bb1f06d4`  
		Last Modified: Fri, 24 Apr 2020 22:02:13 GMT  
		Size: 129.1 MB (129109796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f164ba21e17cf867efb556e534bfdaf30d58988e36de4424ccedc5842f259579`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494c387442cc32b84937ca989fb819fa005f0dec31a42f16ef3817c47232c7f`  
		Last Modified: Fri, 24 Apr 2020 22:01:53 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.6-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:25821e16c7c401986caa09fba3be08b103203a1599edaba8cd34366903b4b3e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154693716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9c0f139339bf92dbef6e630dca8acc4265b72752f7d7b37e16786ed8d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:18:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:19:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:19:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:19:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:19:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:19:33 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 16:19:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:19:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:19:37 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:37 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 16:19:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:20:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:20:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:20:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:20:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:20:11 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:20:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8d1af89634c78002ec70ef345dd88801eff1bbca938f85fc7472acf873b32`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03832d333b77fecdaaf76768c24a0c6797373a576bd7fb9abc41f3e3e5e2e4`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 2.7 MB (2675928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6736a2d19b775007ab26e1c72ee2e84911c375eec60ec697fe5e8deca69f`  
		Last Modified: Fri, 24 Apr 2020 16:21:44 GMT  
		Size: 5.3 MB (5345352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aac5b0c675d956885986db6ac84f954ff2f6a98df26a133ae89ae619cd5be`  
		Last Modified: Fri, 24 Apr 2020 16:21:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53bf51618735c85e240ace69cf43a38a4077593fb9b4633fc1d85d2e655016`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296ff1757ed119711f3cc049cb72f1f77178850e6ba2efc6cb0d1e9e1687bdf`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697b84404da018afccd718c3454ed04a6ee05110f0d573a5d73e25a5c5cd75c`  
		Last Modified: Fri, 24 Apr 2020 16:22:09 GMT  
		Size: 122.9 MB (122907968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458af224982cf3028e9a2a89e362caa3e795382c0448adc60b4ab96bedbcc1ef`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7506dcffce0af812ecd82776f582f438856fd75e7f948fa2a689a841eaf272e0`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.6-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:9a853858232155d691db93ab8ab614ad4636f9465aaab10dad522c6ffdbb6fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160626574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6080841c0f9e130ab30d755a2610d8101b8b45a55cfbce1852edce8e90e15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:34:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 07:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:34:51 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 07:34:51 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 07:35:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 07:35:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 07:35:03 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 07:35:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 07:35:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 07:35:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 07:35:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 07:35:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 07:35:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:35:39 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 07:35:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c464d6728e9ac439c8d2dc10a88d64a54c34ac50926c66cb7b6d12e37b15d6`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd364a38efacff4956ad8e4082d7fa9593aa0a036757fdfbe97487eb26ea2c9`  
		Last Modified: Fri, 24 Apr 2020 07:36:03 GMT  
		Size: 2.7 MB (2714610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e788a62ef53016c8add2417fa25e2141e1b7293acd648f26ed2ddffd54e605b`  
		Last Modified: Fri, 24 Apr 2020 07:36:02 GMT  
		Size: 5.7 MB (5744825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e103dac172d8152c577b2075cc90e6b674188775064cccfbbbc84d93979b3e56`  
		Last Modified: Fri, 24 Apr 2020 07:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fb52c1ef634a5a074adebdaa3f4fc95e636e570c5719c5d662babed85392e`  
		Last Modified: Fri, 24 Apr 2020 07:35:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f95c28bb62ddcdbb79cc6870d5cd9701c912a6307bde4c657e1d0c619430fab`  
		Last Modified: Fri, 24 Apr 2020 07:35:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cea8c1238e8ec47654f290d7a566d006d9302762e741316cd236b909d4577d`  
		Last Modified: Fri, 24 Apr 2020 07:36:18 GMT  
		Size: 126.8 MB (126756767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873535c8ae6f6827fe3d880ab25b1cc404dc3b74898d2ca9bff17136b83caba`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d64c0289b5d5c3ee9e04955ed738543e81fdae4e1a43328fd4d88be18d402b`  
		Last Modified: Fri, 24 Apr 2020 07:36:30 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.6-windowsservercore`

```console
$ docker pull mongo@sha256:7986f24675f34cfc523779ad2f529adb694caa72790836da2ce5169967c79991
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2.6-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.6-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:2617684e95c344a22141b15f413f83531aaa3cb64ec8026f12e9ccd8121755fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2.6-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:58f10c09128d2b379864ecb59d3e59b7b7b0d900c6a3294b4ee7e2dcd61fe4eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4.2.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:a89b09e8bc3153c5c87c52e36a7b6f992ee874c5329cc631e5d9542bf1cbfe31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:8c48baa1571469d7f5ae6d603b92b8027ada5eb39826c009cb33a13b46864908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164649492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3daf8637573f4568ba35ee0f818aa25384f547b6e9cfa0c9bf39b92d5a63da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:59:56 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 22:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 22:00:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 22:00:13 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 22:00:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 22:00:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 22:00:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 22:00:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 22:00:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 22:00:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 22:00:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 22:00:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 22:00:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 22:00:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 22:00:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 22:00:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 22:00:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 22:00:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d269900d94133efa09999e6bd3a64fc1f1ae303aa6a6196b82e8b39582d8a9`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2526abb80afdbc05f3785f8463ca88c113aa9028af96d085ea269cf7e601eb`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 3.0 MB (2981995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eece1f39ec6168fc3e4aaf7860fbeeb79e098e0df5d69b98f3612e65c48735`  
		Last Modified: Fri, 24 Apr 2020 22:01:56 GMT  
		Size: 5.8 MB (5823765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ed78d3204b906dde21c66c4f1c1008483ddd7ebdc6b86ba4e8b41c320fd4f`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a878b8604aebf98b3bc70ccfddeb849aefb3af253a340406b874a1a7f4e6442`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde03a2883d0ac5b63b567bc10a14f01eac2b63396f6fdeff8caed2eb3d25df7`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe534daa349b7d8b4a3eee9920bfa77e5a067f6c8698d81419fde9bb1f06d4`  
		Last Modified: Fri, 24 Apr 2020 22:02:13 GMT  
		Size: 129.1 MB (129109796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f164ba21e17cf867efb556e534bfdaf30d58988e36de4424ccedc5842f259579`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494c387442cc32b84937ca989fb819fa005f0dec31a42f16ef3817c47232c7f`  
		Last Modified: Fri, 24 Apr 2020 22:01:53 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:25821e16c7c401986caa09fba3be08b103203a1599edaba8cd34366903b4b3e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154693716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9c0f139339bf92dbef6e630dca8acc4265b72752f7d7b37e16786ed8d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:18:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:19:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:19:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:19:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:19:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:19:33 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 16:19:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:19:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:19:37 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:37 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 16:19:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:20:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:20:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:20:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:20:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:20:11 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:20:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8d1af89634c78002ec70ef345dd88801eff1bbca938f85fc7472acf873b32`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03832d333b77fecdaaf76768c24a0c6797373a576bd7fb9abc41f3e3e5e2e4`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 2.7 MB (2675928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6736a2d19b775007ab26e1c72ee2e84911c375eec60ec697fe5e8deca69f`  
		Last Modified: Fri, 24 Apr 2020 16:21:44 GMT  
		Size: 5.3 MB (5345352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aac5b0c675d956885986db6ac84f954ff2f6a98df26a133ae89ae619cd5be`  
		Last Modified: Fri, 24 Apr 2020 16:21:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53bf51618735c85e240ace69cf43a38a4077593fb9b4633fc1d85d2e655016`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296ff1757ed119711f3cc049cb72f1f77178850e6ba2efc6cb0d1e9e1687bdf`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697b84404da018afccd718c3454ed04a6ee05110f0d573a5d73e25a5c5cd75c`  
		Last Modified: Fri, 24 Apr 2020 16:22:09 GMT  
		Size: 122.9 MB (122907968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458af224982cf3028e9a2a89e362caa3e795382c0448adc60b4ab96bedbcc1ef`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7506dcffce0af812ecd82776f582f438856fd75e7f948fa2a689a841eaf272e0`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:9a853858232155d691db93ab8ab614ad4636f9465aaab10dad522c6ffdbb6fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160626574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6080841c0f9e130ab30d755a2610d8101b8b45a55cfbce1852edce8e90e15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:34:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 07:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:34:51 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 07:34:51 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 07:35:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 07:35:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 07:35:03 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 07:35:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 07:35:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 07:35:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 07:35:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 07:35:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 07:35:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:35:39 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 07:35:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c464d6728e9ac439c8d2dc10a88d64a54c34ac50926c66cb7b6d12e37b15d6`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd364a38efacff4956ad8e4082d7fa9593aa0a036757fdfbe97487eb26ea2c9`  
		Last Modified: Fri, 24 Apr 2020 07:36:03 GMT  
		Size: 2.7 MB (2714610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e788a62ef53016c8add2417fa25e2141e1b7293acd648f26ed2ddffd54e605b`  
		Last Modified: Fri, 24 Apr 2020 07:36:02 GMT  
		Size: 5.7 MB (5744825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e103dac172d8152c577b2075cc90e6b674188775064cccfbbbc84d93979b3e56`  
		Last Modified: Fri, 24 Apr 2020 07:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fb52c1ef634a5a074adebdaa3f4fc95e636e570c5719c5d662babed85392e`  
		Last Modified: Fri, 24 Apr 2020 07:35:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f95c28bb62ddcdbb79cc6870d5cd9701c912a6307bde4c657e1d0c619430fab`  
		Last Modified: Fri, 24 Apr 2020 07:35:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cea8c1238e8ec47654f290d7a566d006d9302762e741316cd236b909d4577d`  
		Last Modified: Fri, 24 Apr 2020 07:36:18 GMT  
		Size: 126.8 MB (126756767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873535c8ae6f6827fe3d880ab25b1cc404dc3b74898d2ca9bff17136b83caba`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d64c0289b5d5c3ee9e04955ed738543e81fdae4e1a43328fd4d88be18d402b`  
		Last Modified: Fri, 24 Apr 2020 07:36:30 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:7986f24675f34cfc523779ad2f529adb694caa72790836da2ce5169967c79991
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:2617684e95c344a22141b15f413f83531aaa3cb64ec8026f12e9ccd8121755fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:58f10c09128d2b379864ecb59d3e59b7b7b0d900c6a3294b4ee7e2dcd61fe4eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:a89b09e8bc3153c5c87c52e36a7b6f992ee874c5329cc631e5d9542bf1cbfe31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:8c48baa1571469d7f5ae6d603b92b8027ada5eb39826c009cb33a13b46864908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164649492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3daf8637573f4568ba35ee0f818aa25384f547b6e9cfa0c9bf39b92d5a63da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:59:56 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 22:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 22:00:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 22:00:13 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 22:00:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 22:00:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 22:00:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 22:00:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 22:00:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 22:00:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 22:00:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 22:00:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 22:00:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 22:00:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 22:00:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 22:00:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 22:00:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 22:00:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d269900d94133efa09999e6bd3a64fc1f1ae303aa6a6196b82e8b39582d8a9`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2526abb80afdbc05f3785f8463ca88c113aa9028af96d085ea269cf7e601eb`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 3.0 MB (2981995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eece1f39ec6168fc3e4aaf7860fbeeb79e098e0df5d69b98f3612e65c48735`  
		Last Modified: Fri, 24 Apr 2020 22:01:56 GMT  
		Size: 5.8 MB (5823765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ed78d3204b906dde21c66c4f1c1008483ddd7ebdc6b86ba4e8b41c320fd4f`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a878b8604aebf98b3bc70ccfddeb849aefb3af253a340406b874a1a7f4e6442`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde03a2883d0ac5b63b567bc10a14f01eac2b63396f6fdeff8caed2eb3d25df7`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe534daa349b7d8b4a3eee9920bfa77e5a067f6c8698d81419fde9bb1f06d4`  
		Last Modified: Fri, 24 Apr 2020 22:02:13 GMT  
		Size: 129.1 MB (129109796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f164ba21e17cf867efb556e534bfdaf30d58988e36de4424ccedc5842f259579`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494c387442cc32b84937ca989fb819fa005f0dec31a42f16ef3817c47232c7f`  
		Last Modified: Fri, 24 Apr 2020 22:01:53 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:25821e16c7c401986caa09fba3be08b103203a1599edaba8cd34366903b4b3e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154693716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9c0f139339bf92dbef6e630dca8acc4265b72752f7d7b37e16786ed8d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:18:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:19:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:19:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:19:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:19:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:19:33 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 16:19:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:19:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:19:37 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:37 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 16:19:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:20:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:20:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:20:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:20:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:20:11 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:20:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8d1af89634c78002ec70ef345dd88801eff1bbca938f85fc7472acf873b32`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03832d333b77fecdaaf76768c24a0c6797373a576bd7fb9abc41f3e3e5e2e4`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 2.7 MB (2675928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6736a2d19b775007ab26e1c72ee2e84911c375eec60ec697fe5e8deca69f`  
		Last Modified: Fri, 24 Apr 2020 16:21:44 GMT  
		Size: 5.3 MB (5345352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aac5b0c675d956885986db6ac84f954ff2f6a98df26a133ae89ae619cd5be`  
		Last Modified: Fri, 24 Apr 2020 16:21:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53bf51618735c85e240ace69cf43a38a4077593fb9b4633fc1d85d2e655016`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296ff1757ed119711f3cc049cb72f1f77178850e6ba2efc6cb0d1e9e1687bdf`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697b84404da018afccd718c3454ed04a6ee05110f0d573a5d73e25a5c5cd75c`  
		Last Modified: Fri, 24 Apr 2020 16:22:09 GMT  
		Size: 122.9 MB (122907968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458af224982cf3028e9a2a89e362caa3e795382c0448adc60b4ab96bedbcc1ef`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7506dcffce0af812ecd82776f582f438856fd75e7f948fa2a689a841eaf272e0`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:9a853858232155d691db93ab8ab614ad4636f9465aaab10dad522c6ffdbb6fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160626574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6080841c0f9e130ab30d755a2610d8101b8b45a55cfbce1852edce8e90e15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:34:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 07:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:34:51 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 07:34:51 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 07:35:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 07:35:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 07:35:03 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 07:35:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 07:35:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 07:35:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 07:35:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 07:35:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 07:35:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:35:39 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 07:35:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c464d6728e9ac439c8d2dc10a88d64a54c34ac50926c66cb7b6d12e37b15d6`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd364a38efacff4956ad8e4082d7fa9593aa0a036757fdfbe97487eb26ea2c9`  
		Last Modified: Fri, 24 Apr 2020 07:36:03 GMT  
		Size: 2.7 MB (2714610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e788a62ef53016c8add2417fa25e2141e1b7293acd648f26ed2ddffd54e605b`  
		Last Modified: Fri, 24 Apr 2020 07:36:02 GMT  
		Size: 5.7 MB (5744825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e103dac172d8152c577b2075cc90e6b674188775064cccfbbbc84d93979b3e56`  
		Last Modified: Fri, 24 Apr 2020 07:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fb52c1ef634a5a074adebdaa3f4fc95e636e570c5719c5d662babed85392e`  
		Last Modified: Fri, 24 Apr 2020 07:35:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f95c28bb62ddcdbb79cc6870d5cd9701c912a6307bde4c657e1d0c619430fab`  
		Last Modified: Fri, 24 Apr 2020 07:35:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cea8c1238e8ec47654f290d7a566d006d9302762e741316cd236b909d4577d`  
		Last Modified: Fri, 24 Apr 2020 07:36:18 GMT  
		Size: 126.8 MB (126756767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873535c8ae6f6827fe3d880ab25b1cc404dc3b74898d2ca9bff17136b83caba`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d64c0289b5d5c3ee9e04955ed738543e81fdae4e1a43328fd4d88be18d402b`  
		Last Modified: Fri, 24 Apr 2020 07:36:30 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:7986f24675f34cfc523779ad2f529adb694caa72790836da2ce5169967c79991
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:2617684e95c344a22141b15f413f83531aaa3cb64ec8026f12e9ccd8121755fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:58f10c09128d2b379864ecb59d3e59b7b7b0d900c6a3294b4ee7e2dcd61fe4eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:a89b09e8bc3153c5c87c52e36a7b6f992ee874c5329cc631e5d9542bf1cbfe31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:8c48baa1571469d7f5ae6d603b92b8027ada5eb39826c009cb33a13b46864908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164649492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3daf8637573f4568ba35ee0f818aa25384f547b6e9cfa0c9bf39b92d5a63da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:59:56 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 22:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 22:00:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 22:00:13 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 22:00:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 22:00:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 22:00:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 22:00:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 22:00:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 22:00:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 22:00:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 22:00:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 22:00:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 22:00:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 22:00:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 22:00:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 22:00:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 22:00:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d269900d94133efa09999e6bd3a64fc1f1ae303aa6a6196b82e8b39582d8a9`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2526abb80afdbc05f3785f8463ca88c113aa9028af96d085ea269cf7e601eb`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 3.0 MB (2981995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eece1f39ec6168fc3e4aaf7860fbeeb79e098e0df5d69b98f3612e65c48735`  
		Last Modified: Fri, 24 Apr 2020 22:01:56 GMT  
		Size: 5.8 MB (5823765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ed78d3204b906dde21c66c4f1c1008483ddd7ebdc6b86ba4e8b41c320fd4f`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a878b8604aebf98b3bc70ccfddeb849aefb3af253a340406b874a1a7f4e6442`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde03a2883d0ac5b63b567bc10a14f01eac2b63396f6fdeff8caed2eb3d25df7`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe534daa349b7d8b4a3eee9920bfa77e5a067f6c8698d81419fde9bb1f06d4`  
		Last Modified: Fri, 24 Apr 2020 22:02:13 GMT  
		Size: 129.1 MB (129109796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f164ba21e17cf867efb556e534bfdaf30d58988e36de4424ccedc5842f259579`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494c387442cc32b84937ca989fb819fa005f0dec31a42f16ef3817c47232c7f`  
		Last Modified: Fri, 24 Apr 2020 22:01:53 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:25821e16c7c401986caa09fba3be08b103203a1599edaba8cd34366903b4b3e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154693716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9c0f139339bf92dbef6e630dca8acc4265b72752f7d7b37e16786ed8d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:18:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:19:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:19:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:19:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:19:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:19:33 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 16:19:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:19:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:19:37 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:37 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 16:19:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:20:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:20:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:20:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:20:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:20:11 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:20:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8d1af89634c78002ec70ef345dd88801eff1bbca938f85fc7472acf873b32`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03832d333b77fecdaaf76768c24a0c6797373a576bd7fb9abc41f3e3e5e2e4`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 2.7 MB (2675928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6736a2d19b775007ab26e1c72ee2e84911c375eec60ec697fe5e8deca69f`  
		Last Modified: Fri, 24 Apr 2020 16:21:44 GMT  
		Size: 5.3 MB (5345352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aac5b0c675d956885986db6ac84f954ff2f6a98df26a133ae89ae619cd5be`  
		Last Modified: Fri, 24 Apr 2020 16:21:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53bf51618735c85e240ace69cf43a38a4077593fb9b4633fc1d85d2e655016`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296ff1757ed119711f3cc049cb72f1f77178850e6ba2efc6cb0d1e9e1687bdf`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697b84404da018afccd718c3454ed04a6ee05110f0d573a5d73e25a5c5cd75c`  
		Last Modified: Fri, 24 Apr 2020 16:22:09 GMT  
		Size: 122.9 MB (122907968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458af224982cf3028e9a2a89e362caa3e795382c0448adc60b4ab96bedbcc1ef`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7506dcffce0af812ecd82776f582f438856fd75e7f948fa2a689a841eaf272e0`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:9a853858232155d691db93ab8ab614ad4636f9465aaab10dad522c6ffdbb6fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160626574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6080841c0f9e130ab30d755a2610d8101b8b45a55cfbce1852edce8e90e15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:34:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 07:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:34:51 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 07:34:51 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 07:35:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 07:35:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 07:35:03 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 07:35:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 07:35:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 07:35:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 07:35:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 07:35:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 07:35:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:35:39 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 07:35:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c464d6728e9ac439c8d2dc10a88d64a54c34ac50926c66cb7b6d12e37b15d6`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd364a38efacff4956ad8e4082d7fa9593aa0a036757fdfbe97487eb26ea2c9`  
		Last Modified: Fri, 24 Apr 2020 07:36:03 GMT  
		Size: 2.7 MB (2714610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e788a62ef53016c8add2417fa25e2141e1b7293acd648f26ed2ddffd54e605b`  
		Last Modified: Fri, 24 Apr 2020 07:36:02 GMT  
		Size: 5.7 MB (5744825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e103dac172d8152c577b2075cc90e6b674188775064cccfbbbc84d93979b3e56`  
		Last Modified: Fri, 24 Apr 2020 07:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fb52c1ef634a5a074adebdaa3f4fc95e636e570c5719c5d662babed85392e`  
		Last Modified: Fri, 24 Apr 2020 07:35:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f95c28bb62ddcdbb79cc6870d5cd9701c912a6307bde4c657e1d0c619430fab`  
		Last Modified: Fri, 24 Apr 2020 07:35:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cea8c1238e8ec47654f290d7a566d006d9302762e741316cd236b909d4577d`  
		Last Modified: Fri, 24 Apr 2020 07:36:18 GMT  
		Size: 126.8 MB (126756767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873535c8ae6f6827fe3d880ab25b1cc404dc3b74898d2ca9bff17136b83caba`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d64c0289b5d5c3ee9e04955ed738543e81fdae4e1a43328fd4d88be18d402b`  
		Last Modified: Fri, 24 Apr 2020 07:36:30 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:c880f6b56f443bb4d01baa759883228cd84fa8d78fa1a36001d1c0a0712b5a07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:8c48baa1571469d7f5ae6d603b92b8027ada5eb39826c009cb33a13b46864908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164649492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3daf8637573f4568ba35ee0f818aa25384f547b6e9cfa0c9bf39b92d5a63da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 21:59:56 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 22:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 22:00:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 22:00:13 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 22:00:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 22:00:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 22:00:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 22:00:27 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 22:00:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 22:00:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 22:00:28 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 22:00:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 22:00:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 22:00:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 22:00:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 22:00:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 22:00:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 22:00:49 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 22:00:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d269900d94133efa09999e6bd3a64fc1f1ae303aa6a6196b82e8b39582d8a9`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2526abb80afdbc05f3785f8463ca88c113aa9028af96d085ea269cf7e601eb`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 3.0 MB (2981995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3eece1f39ec6168fc3e4aaf7860fbeeb79e098e0df5d69b98f3612e65c48735`  
		Last Modified: Fri, 24 Apr 2020 22:01:56 GMT  
		Size: 5.8 MB (5823765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ed78d3204b906dde21c66c4f1c1008483ddd7ebdc6b86ba4e8b41c320fd4f`  
		Last Modified: Fri, 24 Apr 2020 22:01:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a878b8604aebf98b3bc70ccfddeb849aefb3af253a340406b874a1a7f4e6442`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde03a2883d0ac5b63b567bc10a14f01eac2b63396f6fdeff8caed2eb3d25df7`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe534daa349b7d8b4a3eee9920bfa77e5a067f6c8698d81419fde9bb1f06d4`  
		Last Modified: Fri, 24 Apr 2020 22:02:13 GMT  
		Size: 129.1 MB (129109796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f164ba21e17cf867efb556e534bfdaf30d58988e36de4424ccedc5842f259579`  
		Last Modified: Fri, 24 Apr 2020 22:01:54 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494c387442cc32b84937ca989fb819fa005f0dec31a42f16ef3817c47232c7f`  
		Last Modified: Fri, 24 Apr 2020 22:01:53 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:25821e16c7c401986caa09fba3be08b103203a1599edaba8cd34366903b4b3e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154693716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9c0f139339bf92dbef6e630dca8acc4265b72752f7d7b37e16786ed8d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:18:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 16:19:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:19:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 16:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 16:19:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 16:19:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 16:19:33 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 16:19:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 16:19:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 16:19:37 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:37 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 16:19:38 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 16:19:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 16:20:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 16:20:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 16:20:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 16:20:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 16:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 16:20:11 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 16:20:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8d1af89634c78002ec70ef345dd88801eff1bbca938f85fc7472acf873b32`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03832d333b77fecdaaf76768c24a0c6797373a576bd7fb9abc41f3e3e5e2e4`  
		Last Modified: Fri, 24 Apr 2020 16:21:43 GMT  
		Size: 2.7 MB (2675928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6736a2d19b775007ab26e1c72ee2e84911c375eec60ec697fe5e8deca69f`  
		Last Modified: Fri, 24 Apr 2020 16:21:44 GMT  
		Size: 5.3 MB (5345352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aac5b0c675d956885986db6ac84f954ff2f6a98df26a133ae89ae619cd5be`  
		Last Modified: Fri, 24 Apr 2020 16:21:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53bf51618735c85e240ace69cf43a38a4077593fb9b4633fc1d85d2e655016`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296ff1757ed119711f3cc049cb72f1f77178850e6ba2efc6cb0d1e9e1687bdf`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697b84404da018afccd718c3454ed04a6ee05110f0d573a5d73e25a5c5cd75c`  
		Last Modified: Fri, 24 Apr 2020 16:22:09 GMT  
		Size: 122.9 MB (122907968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458af224982cf3028e9a2a89e362caa3e795382c0448adc60b4ab96bedbcc1ef`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7506dcffce0af812ecd82776f582f438856fd75e7f948fa2a689a841eaf272e0`  
		Last Modified: Fri, 24 Apr 2020 16:21:41 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:9a853858232155d691db93ab8ab614ad4636f9465aaab10dad522c6ffdbb6fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160626574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6080841c0f9e130ab30d755a2610d8101b8b45a55cfbce1852edce8e90e15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:34:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 24 Apr 2020 07:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:34:51 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Apr 2020 07:34:51 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 24 Apr 2020 07:35:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Apr 2020 07:35:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Apr 2020 07:35:03 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 24 Apr 2020 07:35:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 24 Apr 2020 07:35:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_MAJOR=4.2
# Fri, 24 Apr 2020 07:35:11 GMT
ENV MONGO_VERSION=4.2.6
# Fri, 24 Apr 2020 07:35:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 24 Apr 2020 07:35:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 24 Apr 2020 07:35:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 24 Apr 2020 07:35:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 24 Apr 2020 07:35:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:35:39 GMT
EXPOSE 27017
# Fri, 24 Apr 2020 07:35:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c464d6728e9ac439c8d2dc10a88d64a54c34ac50926c66cb7b6d12e37b15d6`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd364a38efacff4956ad8e4082d7fa9593aa0a036757fdfbe97487eb26ea2c9`  
		Last Modified: Fri, 24 Apr 2020 07:36:03 GMT  
		Size: 2.7 MB (2714610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e788a62ef53016c8add2417fa25e2141e1b7293acd648f26ed2ddffd54e605b`  
		Last Modified: Fri, 24 Apr 2020 07:36:02 GMT  
		Size: 5.7 MB (5744825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e103dac172d8152c577b2075cc90e6b674188775064cccfbbbc84d93979b3e56`  
		Last Modified: Fri, 24 Apr 2020 07:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fb52c1ef634a5a074adebdaa3f4fc95e636e570c5719c5d662babed85392e`  
		Last Modified: Fri, 24 Apr 2020 07:35:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f95c28bb62ddcdbb79cc6870d5cd9701c912a6307bde4c657e1d0c619430fab`  
		Last Modified: Fri, 24 Apr 2020 07:35:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cea8c1238e8ec47654f290d7a566d006d9302762e741316cd236b909d4577d`  
		Last Modified: Fri, 24 Apr 2020 07:36:18 GMT  
		Size: 126.8 MB (126756767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873535c8ae6f6827fe3d880ab25b1cc404dc3b74898d2ca9bff17136b83caba`  
		Last Modified: Fri, 24 Apr 2020 07:36:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d64c0289b5d5c3ee9e04955ed738543e81fdae4e1a43328fd4d88be18d402b`  
		Last Modified: Fri, 24 Apr 2020 07:36:30 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:7986f24675f34cfc523779ad2f529adb694caa72790836da2ce5169967c79991
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:2617684e95c344a22141b15f413f83531aaa3cb64ec8026f12e9ccd8121755fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:58f10c09128d2b379864ecb59d3e59b7b7b0d900c6a3294b4ee7e2dcd61fe4eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:e7fd976e7ab5921662175ee9474a5baf7e5b38ccc852203f0306f72269a5957b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828575320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95b778853d3c96149981e511cc7945a56fb3ea18a19d12f21ae77a623a5e61a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:16:47 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:16:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:16:49 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:33:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:33:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:33:32 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:33:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6820df30287c85ecafda66047b2abebde529eb43bda3a776e1c8edbf594daa1a`  
		Last Modified: Wed, 13 May 2020 21:18:09 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f1c345979075873ace9494da3f4de4ed0aa9d980755016c84f19cfc6ca6d`  
		Last Modified: Wed, 13 May 2020 21:18:08 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4cf92e7a5818b417d2b90e32b11103aab377cff8c368fbc673c67b7f4c572e`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e58d4acdc2527a0bfd2bc348bf49e27ea9e24f6bbb27684246c7d9e2aae29ee`  
		Last Modified: Wed, 13 May 2020 21:18:30 GMT  
		Size: 96.7 MB (96677362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a9081cd9bbf14f7e8a2cadff80bc61e45ee1cbb14bdc98046723e982b24e0`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e3c44e866b92480681f47bd84e45ec5aef34f4c8aaa8be2922faed53fa31b1`  
		Last Modified: Wed, 13 May 2020 21:18:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8d9460c4e0dfadd979d895217399cf4fae10118ca05fcc143ae253f3e1096c`  
		Last Modified: Wed, 13 May 2020 21:18:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
