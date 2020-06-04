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
-	[`mongo:4.2.7`](#mongo427)
-	[`mongo:4.2.7-bionic`](#mongo427-bionic)
-	[`mongo:4.2.7-windowsservercore`](#mongo427-windowsservercore)
-	[`mongo:4.2.7-windowsservercore-1809`](#mongo427-windowsservercore-1809)
-	[`mongo:4.2.7-windowsservercore-ltsc2016`](#mongo427-windowsservercore-ltsc2016)
-	[`mongo:4.2-bionic`](#mongo42-bionic)
-	[`mongo:4.2-windowsservercore`](#mongo42-windowsservercore)
-	[`mongo:4.2-windowsservercore-1809`](#mongo42-windowsservercore-1809)
-	[`mongo:4.2-windowsservercore-ltsc2016`](#mongo42-windowsservercore-ltsc2016)
-	[`mongo:4.4.0-rc8`](#mongo440-rc8)
-	[`mongo:4.4.0-rc8-bionic`](#mongo440-rc8-bionic)
-	[`mongo:4.4.0-rc8-windowsservercore`](#mongo440-rc8-windowsservercore)
-	[`mongo:4.4.0-rc8-windowsservercore-1809`](#mongo440-rc8-windowsservercore-1809)
-	[`mongo:4.4.0-rc8-windowsservercore-ltsc2016`](#mongo440-rc8-windowsservercore-ltsc2016)
-	[`mongo:4.4-rc`](#mongo44-rc)
-	[`mongo:4.4-rc-bionic`](#mongo44-rc-bionic)
-	[`mongo:4.4-rc-windowsservercore`](#mongo44-rc-windowsservercore)
-	[`mongo:4.4-rc-windowsservercore-1809`](#mongo44-rc-windowsservercore-1809)
-	[`mongo:4.4-rc-windowsservercore-ltsc2016`](#mongo44-rc-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:be8d903a68997dd63f64479004a7eeb4f0674dde7ab3cbd1145e5658da3a817b
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
$ docker pull mongo@sha256:bd251a06b6423d0c37d37de1e19899b2d7b861df43d1b737b274cc95ac913885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164653603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68b650ad44f7a95c256ad2df5c40fbc3b13001f36ac7b7cd25f5f9a09be7d`
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
# Tue, 26 May 2020 22:37:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:37:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:37:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:37:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:37:52 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:37:53 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:37:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:37:53 GMT
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
	-	`sha256:978c572f04400f6e66309862a870a43ad987aadbb83dde6bf69aa704bd825175`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a600ffcf6a6cacd0d3e0eafddf0fa470759c45d3c11aebfb148c821f5ae66b`  
		Last Modified: Tue, 26 May 2020 22:40:51 GMT  
		Size: 129.1 MB (129113906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f812cdfe69fa174869fbf3ec347c097ac7db9f0ebe95263f818c27638c533`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8109e271104450b0ab84c81eb31ee3345711d7d41b35610029c44d15311dc9`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b8f41e6ed567bbb68d5cdb364664eef7c5f4f9bb628d25bb71fe1a532aea7856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154691636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580631906251de3ae7da70cd333fae9886d964e7e30d39e65b55c24a77093843`
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
# Tue, 26 May 2020 22:01:49 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:01:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:02:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:02:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:02:43 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:02:45 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:02:48 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:02:51 GMT
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
	-	`sha256:1ee6871420084682cb152ede4fb479d89174a0e623e68b93cfd21412586093b7`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23903f79dae06f8cc3aa422bb9893de8fcf91e92a504d05db484e34a0efbb91d`  
		Last Modified: Tue, 26 May 2020 22:03:45 GMT  
		Size: 122.9 MB (122905885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec235da2971da8b9af665d6caff32c9122bc5112a4c7280c57bd65f0283c2807`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac5d2db76761538d764cac5f29378ec6fdb214380caeb74730e620f2fbe529c`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:5d4da8f703443f19b3b0665a5e5922c5e349c2d2beaf88cd629db7faa0b3729f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160608601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a7890bfca6b2ee342feb02c588fd72bc4a84cf9c887a0d0647c9f92dcb4278`
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
# Tue, 26 May 2020 21:45:43 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 21:45:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 21:46:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 21:46:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 21:46:35 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 21:46:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 21:46:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 21:46:36 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:37 GMT
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
	-	`sha256:a211607bd79c344a64bd1823730cf4ff32c204005a9c31f6043d78322cfec773`  
		Last Modified: Tue, 26 May 2020 21:46:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358fcf8acc5b9c5439f270d6d7937fa6e3066ba8663568e4fcab9ce23fc7ffa7`  
		Last Modified: Tue, 26 May 2020 21:47:36 GMT  
		Size: 126.7 MB (126738794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba3c21f431df187bacc529912e2abec012ebc9d946e50ab3fed60a02bd3fbd`  
		Last Modified: Tue, 26 May 2020 21:47:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68d35b3abc69df8615e4bb3acec1fb6488e1c184b2c94d556cd5d47cc3fa46`  
		Last Modified: Tue, 26 May 2020 21:46:54 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull mongo@sha256:be8d903a68997dd63f64479004a7eeb4f0674dde7ab3cbd1145e5658da3a817b
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
$ docker pull mongo@sha256:bd251a06b6423d0c37d37de1e19899b2d7b861df43d1b737b274cc95ac913885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164653603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68b650ad44f7a95c256ad2df5c40fbc3b13001f36ac7b7cd25f5f9a09be7d`
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
# Tue, 26 May 2020 22:37:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:37:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:37:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:37:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:37:52 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:37:53 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:37:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:37:53 GMT
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
	-	`sha256:978c572f04400f6e66309862a870a43ad987aadbb83dde6bf69aa704bd825175`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a600ffcf6a6cacd0d3e0eafddf0fa470759c45d3c11aebfb148c821f5ae66b`  
		Last Modified: Tue, 26 May 2020 22:40:51 GMT  
		Size: 129.1 MB (129113906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f812cdfe69fa174869fbf3ec347c097ac7db9f0ebe95263f818c27638c533`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8109e271104450b0ab84c81eb31ee3345711d7d41b35610029c44d15311dc9`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b8f41e6ed567bbb68d5cdb364664eef7c5f4f9bb628d25bb71fe1a532aea7856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154691636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580631906251de3ae7da70cd333fae9886d964e7e30d39e65b55c24a77093843`
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
# Tue, 26 May 2020 22:01:49 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:01:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:02:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:02:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:02:43 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:02:45 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:02:48 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:02:51 GMT
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
	-	`sha256:1ee6871420084682cb152ede4fb479d89174a0e623e68b93cfd21412586093b7`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23903f79dae06f8cc3aa422bb9893de8fcf91e92a504d05db484e34a0efbb91d`  
		Last Modified: Tue, 26 May 2020 22:03:45 GMT  
		Size: 122.9 MB (122905885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec235da2971da8b9af665d6caff32c9122bc5112a4c7280c57bd65f0283c2807`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac5d2db76761538d764cac5f29378ec6fdb214380caeb74730e620f2fbe529c`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; s390x

```console
$ docker pull mongo@sha256:5d4da8f703443f19b3b0665a5e5922c5e349c2d2beaf88cd629db7faa0b3729f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160608601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a7890bfca6b2ee342feb02c588fd72bc4a84cf9c887a0d0647c9f92dcb4278`
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
# Tue, 26 May 2020 21:45:43 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 21:45:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 21:46:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 21:46:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 21:46:35 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 21:46:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 21:46:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 21:46:36 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:37 GMT
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
	-	`sha256:a211607bd79c344a64bd1823730cf4ff32c204005a9c31f6043d78322cfec773`  
		Last Modified: Tue, 26 May 2020 21:46:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358fcf8acc5b9c5439f270d6d7937fa6e3066ba8663568e4fcab9ce23fc7ffa7`  
		Last Modified: Tue, 26 May 2020 21:47:36 GMT  
		Size: 126.7 MB (126738794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba3c21f431df187bacc529912e2abec012ebc9d946e50ab3fed60a02bd3fbd`  
		Last Modified: Tue, 26 May 2020 21:47:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68d35b3abc69df8615e4bb3acec1fb6488e1c184b2c94d556cd5d47cc3fa46`  
		Last Modified: Tue, 26 May 2020 21:46:54 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.7`

```console
$ docker pull mongo@sha256:be8d903a68997dd63f64479004a7eeb4f0674dde7ab3cbd1145e5658da3a817b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2.7` - linux; amd64

```console
$ docker pull mongo@sha256:bd251a06b6423d0c37d37de1e19899b2d7b861df43d1b737b274cc95ac913885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164653603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68b650ad44f7a95c256ad2df5c40fbc3b13001f36ac7b7cd25f5f9a09be7d`
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
# Tue, 26 May 2020 22:37:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:37:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:37:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:37:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:37:52 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:37:53 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:37:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:37:53 GMT
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
	-	`sha256:978c572f04400f6e66309862a870a43ad987aadbb83dde6bf69aa704bd825175`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a600ffcf6a6cacd0d3e0eafddf0fa470759c45d3c11aebfb148c821f5ae66b`  
		Last Modified: Tue, 26 May 2020 22:40:51 GMT  
		Size: 129.1 MB (129113906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f812cdfe69fa174869fbf3ec347c097ac7db9f0ebe95263f818c27638c533`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8109e271104450b0ab84c81eb31ee3345711d7d41b35610029c44d15311dc9`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.7` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b8f41e6ed567bbb68d5cdb364664eef7c5f4f9bb628d25bb71fe1a532aea7856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154691636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580631906251de3ae7da70cd333fae9886d964e7e30d39e65b55c24a77093843`
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
# Tue, 26 May 2020 22:01:49 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:01:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:02:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:02:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:02:43 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:02:45 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:02:48 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:02:51 GMT
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
	-	`sha256:1ee6871420084682cb152ede4fb479d89174a0e623e68b93cfd21412586093b7`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23903f79dae06f8cc3aa422bb9893de8fcf91e92a504d05db484e34a0efbb91d`  
		Last Modified: Tue, 26 May 2020 22:03:45 GMT  
		Size: 122.9 MB (122905885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec235da2971da8b9af665d6caff32c9122bc5112a4c7280c57bd65f0283c2807`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac5d2db76761538d764cac5f29378ec6fdb214380caeb74730e620f2fbe529c`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.7` - linux; s390x

```console
$ docker pull mongo@sha256:5d4da8f703443f19b3b0665a5e5922c5e349c2d2beaf88cd629db7faa0b3729f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160608601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a7890bfca6b2ee342feb02c588fd72bc4a84cf9c887a0d0647c9f92dcb4278`
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
# Tue, 26 May 2020 21:45:43 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 21:45:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 21:46:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 21:46:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 21:46:35 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 21:46:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 21:46:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 21:46:36 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:37 GMT
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
	-	`sha256:a211607bd79c344a64bd1823730cf4ff32c204005a9c31f6043d78322cfec773`  
		Last Modified: Tue, 26 May 2020 21:46:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358fcf8acc5b9c5439f270d6d7937fa6e3066ba8663568e4fcab9ce23fc7ffa7`  
		Last Modified: Tue, 26 May 2020 21:47:36 GMT  
		Size: 126.7 MB (126738794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba3c21f431df187bacc529912e2abec012ebc9d946e50ab3fed60a02bd3fbd`  
		Last Modified: Tue, 26 May 2020 21:47:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68d35b3abc69df8615e4bb3acec1fb6488e1c184b2c94d556cd5d47cc3fa46`  
		Last Modified: Tue, 26 May 2020 21:46:54 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.7` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.7` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.7-bionic`

```console
$ docker pull mongo@sha256:9d5a8a478b36f9034b6b6ffca96e4172cacca8d2f0a0c96a5822bc01d518b116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2.7-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:bd251a06b6423d0c37d37de1e19899b2d7b861df43d1b737b274cc95ac913885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164653603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68b650ad44f7a95c256ad2df5c40fbc3b13001f36ac7b7cd25f5f9a09be7d`
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
# Tue, 26 May 2020 22:37:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:37:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:37:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:37:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:37:52 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:37:53 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:37:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:37:53 GMT
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
	-	`sha256:978c572f04400f6e66309862a870a43ad987aadbb83dde6bf69aa704bd825175`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a600ffcf6a6cacd0d3e0eafddf0fa470759c45d3c11aebfb148c821f5ae66b`  
		Last Modified: Tue, 26 May 2020 22:40:51 GMT  
		Size: 129.1 MB (129113906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f812cdfe69fa174869fbf3ec347c097ac7db9f0ebe95263f818c27638c533`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8109e271104450b0ab84c81eb31ee3345711d7d41b35610029c44d15311dc9`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.7-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b8f41e6ed567bbb68d5cdb364664eef7c5f4f9bb628d25bb71fe1a532aea7856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154691636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580631906251de3ae7da70cd333fae9886d964e7e30d39e65b55c24a77093843`
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
# Tue, 26 May 2020 22:01:49 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:01:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:02:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:02:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:02:43 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:02:45 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:02:48 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:02:51 GMT
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
	-	`sha256:1ee6871420084682cb152ede4fb479d89174a0e623e68b93cfd21412586093b7`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23903f79dae06f8cc3aa422bb9893de8fcf91e92a504d05db484e34a0efbb91d`  
		Last Modified: Tue, 26 May 2020 22:03:45 GMT  
		Size: 122.9 MB (122905885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec235da2971da8b9af665d6caff32c9122bc5112a4c7280c57bd65f0283c2807`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac5d2db76761538d764cac5f29378ec6fdb214380caeb74730e620f2fbe529c`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.7-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:5d4da8f703443f19b3b0665a5e5922c5e349c2d2beaf88cd629db7faa0b3729f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160608601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a7890bfca6b2ee342feb02c588fd72bc4a84cf9c887a0d0647c9f92dcb4278`
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
# Tue, 26 May 2020 21:45:43 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 21:45:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 21:46:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 21:46:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 21:46:35 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 21:46:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 21:46:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 21:46:36 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:37 GMT
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
	-	`sha256:a211607bd79c344a64bd1823730cf4ff32c204005a9c31f6043d78322cfec773`  
		Last Modified: Tue, 26 May 2020 21:46:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358fcf8acc5b9c5439f270d6d7937fa6e3066ba8663568e4fcab9ce23fc7ffa7`  
		Last Modified: Tue, 26 May 2020 21:47:36 GMT  
		Size: 126.7 MB (126738794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba3c21f431df187bacc529912e2abec012ebc9d946e50ab3fed60a02bd3fbd`  
		Last Modified: Tue, 26 May 2020 21:47:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68d35b3abc69df8615e4bb3acec1fb6488e1c184b2c94d556cd5d47cc3fa46`  
		Last Modified: Tue, 26 May 2020 21:46:54 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.7-windowsservercore`

```console
$ docker pull mongo@sha256:20055d57fb34769eeab26de814a41c9ecff2c0deff29ff9d523652ac2a0492dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2.7-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.7-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.7-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0768e7755712a5a86421a0aad9801e3b4a46f639e89c231011e92a67bb1e59cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2.7-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.7-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b465214c1a5519ea93ce8e61cf0a33f388b46c157984807f8e596a5665b75ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4.2.7-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:9d5a8a478b36f9034b6b6ffca96e4172cacca8d2f0a0c96a5822bc01d518b116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:bd251a06b6423d0c37d37de1e19899b2d7b861df43d1b737b274cc95ac913885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164653603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68b650ad44f7a95c256ad2df5c40fbc3b13001f36ac7b7cd25f5f9a09be7d`
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
# Tue, 26 May 2020 22:37:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:37:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:37:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:37:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:37:52 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:37:53 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:37:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:37:53 GMT
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
	-	`sha256:978c572f04400f6e66309862a870a43ad987aadbb83dde6bf69aa704bd825175`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a600ffcf6a6cacd0d3e0eafddf0fa470759c45d3c11aebfb148c821f5ae66b`  
		Last Modified: Tue, 26 May 2020 22:40:51 GMT  
		Size: 129.1 MB (129113906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f812cdfe69fa174869fbf3ec347c097ac7db9f0ebe95263f818c27638c533`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8109e271104450b0ab84c81eb31ee3345711d7d41b35610029c44d15311dc9`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b8f41e6ed567bbb68d5cdb364664eef7c5f4f9bb628d25bb71fe1a532aea7856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154691636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580631906251de3ae7da70cd333fae9886d964e7e30d39e65b55c24a77093843`
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
# Tue, 26 May 2020 22:01:49 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:01:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:02:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:02:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:02:43 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:02:45 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:02:48 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:02:51 GMT
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
	-	`sha256:1ee6871420084682cb152ede4fb479d89174a0e623e68b93cfd21412586093b7`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23903f79dae06f8cc3aa422bb9893de8fcf91e92a504d05db484e34a0efbb91d`  
		Last Modified: Tue, 26 May 2020 22:03:45 GMT  
		Size: 122.9 MB (122905885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec235da2971da8b9af665d6caff32c9122bc5112a4c7280c57bd65f0283c2807`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac5d2db76761538d764cac5f29378ec6fdb214380caeb74730e620f2fbe529c`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:5d4da8f703443f19b3b0665a5e5922c5e349c2d2beaf88cd629db7faa0b3729f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160608601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a7890bfca6b2ee342feb02c588fd72bc4a84cf9c887a0d0647c9f92dcb4278`
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
# Tue, 26 May 2020 21:45:43 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 21:45:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 21:46:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 21:46:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 21:46:35 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 21:46:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 21:46:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 21:46:36 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:37 GMT
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
	-	`sha256:a211607bd79c344a64bd1823730cf4ff32c204005a9c31f6043d78322cfec773`  
		Last Modified: Tue, 26 May 2020 21:46:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358fcf8acc5b9c5439f270d6d7937fa6e3066ba8663568e4fcab9ce23fc7ffa7`  
		Last Modified: Tue, 26 May 2020 21:47:36 GMT  
		Size: 126.7 MB (126738794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba3c21f431df187bacc529912e2abec012ebc9d946e50ab3fed60a02bd3fbd`  
		Last Modified: Tue, 26 May 2020 21:47:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68d35b3abc69df8615e4bb3acec1fb6488e1c184b2c94d556cd5d47cc3fa46`  
		Last Modified: Tue, 26 May 2020 21:46:54 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:20055d57fb34769eeab26de814a41c9ecff2c0deff29ff9d523652ac2a0492dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0768e7755712a5a86421a0aad9801e3b4a46f639e89c231011e92a67bb1e59cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b465214c1a5519ea93ce8e61cf0a33f388b46c157984807f8e596a5665b75ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-rc8`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.4.0-rc8-bionic`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.4.0-rc8-windowsservercore`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.4.0-rc8-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.4.0-rc8-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.4-rc`

```console
$ docker pull mongo@sha256:c95747151d8f85632c583e5f6f24b0623759222d43e4bcc02d392c841861d6dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.4-rc` - linux; amd64

```console
$ docker pull mongo@sha256:7959c202806eaeab6bf855d90367730d30253d91477352f2ffb9397831a5cb64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.4 MB (174419181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb3f601e3900fefa3d3ff8a4e15d25a42f84dbebd904de0e91e7408e6472f214`
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
# Wed, 27 May 2020 18:23:29 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 May 2020 18:23:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 May 2020 18:23:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 May 2020 18:23:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:23:32 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:23:32 GMT
ENV MONGO_MAJOR=testing
# Wed, 27 May 2020 18:23:32 GMT
ENV MONGO_VERSION=4.4.0~rc7
# Wed, 27 May 2020 18:23:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 May 2020 18:23:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 May 2020 18:23:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 May 2020 18:23:59 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 May 2020 18:24:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 27 May 2020 18:24:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 May 2020 18:24:00 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:24:00 GMT
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
	-	`sha256:3cf8af686ff7ecad86f79a2a6f56b0e868df82273e54820d24d769e20da85f8f`  
		Last Modified: Wed, 27 May 2020 18:24:17 GMT  
		Size: 6.3 KB (6253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410267caebb8c1f695d0b9d5a31e533c295d070e6b7f5a8dae64d9d2c5cc4a7c`  
		Last Modified: Wed, 27 May 2020 18:24:17 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e300d4bb40bdb5c56e7c371c53d0adcb6fe0acba9cd0a84f58eaa42c6437e4ba`  
		Last Modified: Wed, 27 May 2020 18:24:51 GMT  
		Size: 138.9 MB (138874664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f1b8eb1b13663d7bef7fb54f8e18e378fcdb3a2cb135267861a2e486529aba`  
		Last Modified: Wed, 27 May 2020 18:24:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e926fffb12f532cdd27da01bb2d4bc3f702f419cb52926e3e1710ef93b5caf`  
		Last Modified: Wed, 27 May 2020 18:24:17 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:75797ceedaaf59834db3f464131307726c5e61e4d3240325cc06795d8e4a307e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.4 MB (164401051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3591e78631d9ef3dc8ebade7eeea090dc388e1f7d031f647bfab14f0a387e31`
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
# Wed, 27 May 2020 18:42:53 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 May 2020 18:42:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 May 2020 18:42:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 May 2020 18:42:59 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:43:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:43:00 GMT
ENV MONGO_MAJOR=testing
# Wed, 27 May 2020 18:43:01 GMT
ENV MONGO_VERSION=4.4.0~rc7
# Wed, 27 May 2020 18:43:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 May 2020 18:43:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 May 2020 18:43:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 May 2020 18:43:34 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 May 2020 18:43:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 27 May 2020 18:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 May 2020 18:43:36 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:43:37 GMT
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
	-	`sha256:cb9151d382154969b8b8d28c29ac34ec3161ea390dd72e03c1962eb7eda51bd0`  
		Last Modified: Wed, 27 May 2020 18:44:06 GMT  
		Size: 6.3 KB (6252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5790dae9206792022638e2c1d817ef1fd81400d1197a9f4e5172d9171361c8`  
		Last Modified: Wed, 27 May 2020 18:44:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034c23eb8c94ed4bb3b518fb00d6cebee19b8add59d354639b27bd652fe49223`  
		Last Modified: Wed, 27 May 2020 18:44:39 GMT  
		Size: 132.6 MB (132610485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00cca2df57b948165e9bc8f861fd28b6a85f6c78bd998674ba242dd950ad5dc`  
		Last Modified: Wed, 27 May 2020 18:44:07 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d373532092c356fafd30ff802da50107a464dcce8b4be581d0072325f0eec49`  
		Last Modified: Wed, 27 May 2020 18:44:06 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc` - linux; s390x

```console
$ docker pull mongo@sha256:d400e471bc8a4372c6d8c0a4508db1812b71f2ada14e99c4741707b8ea8ca1f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169466399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:814991d70aacb8c652be04984c5073d4e3c76e5a8b3bf913ce786f5d5c85620e`
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
# Wed, 27 May 2020 18:43:41 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 May 2020 18:43:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 May 2020 18:43:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 May 2020 18:43:46 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:43:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:43:47 GMT
ENV MONGO_MAJOR=testing
# Wed, 27 May 2020 18:43:47 GMT
ENV MONGO_VERSION=4.4.0~rc7
# Wed, 27 May 2020 18:43:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 May 2020 18:44:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 May 2020 18:44:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 May 2020 18:44:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 May 2020 18:44:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 27 May 2020 18:44:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 May 2020 18:44:44 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:44:45 GMT
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
	-	`sha256:ec7bf992a9bc29b09fd8fd3c9124deea05c56142815ba0d4186fa377dced902d`  
		Last Modified: Wed, 27 May 2020 18:45:12 GMT  
		Size: 6.3 KB (6254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08ccafada81bad3283032d9d7fbfe18460ed908886cabfdbaabd59bfa557c17`  
		Last Modified: Wed, 27 May 2020 18:45:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1128b630569efc39861fc39a1bd6b49a1bf3914ef607ea51fd9974d6000d14`  
		Last Modified: Wed, 27 May 2020 18:45:33 GMT  
		Size: 135.6 MB (135591772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7824f1fee1a2f0cd08b56fa89e23b0b6f638011b8c4ef4ea73459421a9e392d7`  
		Last Modified: Wed, 27 May 2020 18:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53634b129038dca0fdd69e092684760357550fe4e2af7a966bc58a6e2fa45bef`  
		Last Modified: Wed, 27 May 2020 18:45:43 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:bd65d37f2b73020adb7e393b6de97b43f488263b8a0664fe2be5d43ffea318ce
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5782737930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0652785d046112fb8b7577d4309b99d566db1c54ecf7da51be1272fc8316c68e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 27 May 2020 18:14:44 GMT
ENV MONGO_VERSION=4.4.0-rc7
# Wed, 27 May 2020 18:14:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc7-signed.msi
# Wed, 27 May 2020 18:14:47 GMT
ENV MONGO_DOWNLOAD_SHA256=2cfcb05237b05c480761421a78126fcc69761e8396c99e222dcd433c0c5230f1
# Wed, 27 May 2020 18:30:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 27 May 2020 18:30:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 May 2020 18:30:37 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:30:38 GMT
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
	-	`sha256:b2152a451adb220520a5fca7a7f5ee9b59a5ee1c5890127e6d4e1513f1a6aeac`  
		Last Modified: Wed, 27 May 2020 18:51:01 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30527b5ff54f875584fc15d7ca1395fe3615b50fecc76b045bd19977f22f01c`  
		Last Modified: Wed, 27 May 2020 18:51:01 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702fa76eb41d5a6a00c325ada2aaf92a55fcda20232abaa2ccfb38cd0e6b64dd`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850bc1d85a1e940fec81fb23df0f146af25215abf892c9e4aa3920ee178a0240`  
		Last Modified: Wed, 27 May 2020 18:51:09 GMT  
		Size: 50.8 MB (50840027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0cd9a5e90d61da83a3ec185ff9c24055219e2d955317a8551521cf815bff57`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1243585b1cce5c1b0c05d2de35f71db8fbb19681b6fb1f64d6b0efdce529561f`  
		Last Modified: Wed, 27 May 2020 18:50:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f26a4c416d8d54aa9ad4186fed86dfe21d87ab19a8db9ed8659e0bc4841666e`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:70bc30df68902220e386532bf2337912d72b437f1974fec18458621f913acabb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2126230588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769dbe6ef1ce3d8d76060466c0feaa996319767448a3bf90a24e8aced08a75ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 27 May 2020 18:30:47 GMT
ENV MONGO_VERSION=4.4.0-rc7
# Wed, 27 May 2020 18:30:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc7-signed.msi
# Wed, 27 May 2020 18:30:48 GMT
ENV MONGO_DOWNLOAD_SHA256=2cfcb05237b05c480761421a78126fcc69761e8396c99e222dcd433c0c5230f1
# Wed, 27 May 2020 18:49:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 27 May 2020 18:49:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 May 2020 18:49:54 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:49:56 GMT
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
	-	`sha256:fb996e03af1eebd8fd548ac88e3ab9cb3d14b0b643573ca6c92ec319d98cabae`  
		Last Modified: Wed, 27 May 2020 18:51:21 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50dd2e8dc45ae9131283b60d78f26d56b824cf403cda9040c599900441bcfcb4`  
		Last Modified: Wed, 27 May 2020 18:51:21 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7feed001c9cff121f320362b36dc092d9043df9e5c725009867db7f0dcb4668`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e23083c29faa7ef259a9da86e2fc53d4cae2cfa3cf50cef3fdd392dfb5a097b`  
		Last Modified: Wed, 27 May 2020 18:52:15 GMT  
		Size: 407.9 MB (407889623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26005df8dc2749db3ea8a606283c1749ed8b1c49fb48f73e664eaba993663414`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb755abaacde5dc90adbaca2838324e3ae94dcc74f3819110d765b66e44506e8`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f69a4cd6bbf2a72ebb194850174a5672de9de41e8e8c33f1db1ef45445af9c7`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc-bionic`

```console
$ docker pull mongo@sha256:c57ef370abb66f11edf520c54e7e4ddc5a16f1ed50bcd3e80dc78078831415e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-rc-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:7959c202806eaeab6bf855d90367730d30253d91477352f2ffb9397831a5cb64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.4 MB (174419181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb3f601e3900fefa3d3ff8a4e15d25a42f84dbebd904de0e91e7408e6472f214`
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
# Wed, 27 May 2020 18:23:29 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 May 2020 18:23:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 May 2020 18:23:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 May 2020 18:23:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:23:32 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:23:32 GMT
ENV MONGO_MAJOR=testing
# Wed, 27 May 2020 18:23:32 GMT
ENV MONGO_VERSION=4.4.0~rc7
# Wed, 27 May 2020 18:23:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 May 2020 18:23:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 May 2020 18:23:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 May 2020 18:23:59 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 May 2020 18:24:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 27 May 2020 18:24:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 May 2020 18:24:00 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:24:00 GMT
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
	-	`sha256:3cf8af686ff7ecad86f79a2a6f56b0e868df82273e54820d24d769e20da85f8f`  
		Last Modified: Wed, 27 May 2020 18:24:17 GMT  
		Size: 6.3 KB (6253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410267caebb8c1f695d0b9d5a31e533c295d070e6b7f5a8dae64d9d2c5cc4a7c`  
		Last Modified: Wed, 27 May 2020 18:24:17 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e300d4bb40bdb5c56e7c371c53d0adcb6fe0acba9cd0a84f58eaa42c6437e4ba`  
		Last Modified: Wed, 27 May 2020 18:24:51 GMT  
		Size: 138.9 MB (138874664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f1b8eb1b13663d7bef7fb54f8e18e378fcdb3a2cb135267861a2e486529aba`  
		Last Modified: Wed, 27 May 2020 18:24:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e926fffb12f532cdd27da01bb2d4bc3f702f419cb52926e3e1710ef93b5caf`  
		Last Modified: Wed, 27 May 2020 18:24:17 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:75797ceedaaf59834db3f464131307726c5e61e4d3240325cc06795d8e4a307e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.4 MB (164401051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3591e78631d9ef3dc8ebade7eeea090dc388e1f7d031f647bfab14f0a387e31`
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
# Wed, 27 May 2020 18:42:53 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 May 2020 18:42:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 May 2020 18:42:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 May 2020 18:42:59 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:43:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:43:00 GMT
ENV MONGO_MAJOR=testing
# Wed, 27 May 2020 18:43:01 GMT
ENV MONGO_VERSION=4.4.0~rc7
# Wed, 27 May 2020 18:43:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 May 2020 18:43:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 May 2020 18:43:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 May 2020 18:43:34 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 May 2020 18:43:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 27 May 2020 18:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 May 2020 18:43:36 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:43:37 GMT
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
	-	`sha256:cb9151d382154969b8b8d28c29ac34ec3161ea390dd72e03c1962eb7eda51bd0`  
		Last Modified: Wed, 27 May 2020 18:44:06 GMT  
		Size: 6.3 KB (6252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5790dae9206792022638e2c1d817ef1fd81400d1197a9f4e5172d9171361c8`  
		Last Modified: Wed, 27 May 2020 18:44:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034c23eb8c94ed4bb3b518fb00d6cebee19b8add59d354639b27bd652fe49223`  
		Last Modified: Wed, 27 May 2020 18:44:39 GMT  
		Size: 132.6 MB (132610485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00cca2df57b948165e9bc8f861fd28b6a85f6c78bd998674ba242dd950ad5dc`  
		Last Modified: Wed, 27 May 2020 18:44:07 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d373532092c356fafd30ff802da50107a464dcce8b4be581d0072325f0eec49`  
		Last Modified: Wed, 27 May 2020 18:44:06 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:d400e471bc8a4372c6d8c0a4508db1812b71f2ada14e99c4741707b8ea8ca1f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169466399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:814991d70aacb8c652be04984c5073d4e3c76e5a8b3bf913ce786f5d5c85620e`
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
# Wed, 27 May 2020 18:43:41 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 May 2020 18:43:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 May 2020 18:43:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 May 2020 18:43:46 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:43:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 May 2020 18:43:47 GMT
ENV MONGO_MAJOR=testing
# Wed, 27 May 2020 18:43:47 GMT
ENV MONGO_VERSION=4.4.0~rc7
# Wed, 27 May 2020 18:43:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 May 2020 18:44:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 May 2020 18:44:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 May 2020 18:44:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 May 2020 18:44:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 27 May 2020 18:44:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 May 2020 18:44:44 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:44:45 GMT
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
	-	`sha256:ec7bf992a9bc29b09fd8fd3c9124deea05c56142815ba0d4186fa377dced902d`  
		Last Modified: Wed, 27 May 2020 18:45:12 GMT  
		Size: 6.3 KB (6254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08ccafada81bad3283032d9d7fbfe18460ed908886cabfdbaabd59bfa557c17`  
		Last Modified: Wed, 27 May 2020 18:45:12 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1128b630569efc39861fc39a1bd6b49a1bf3914ef607ea51fd9974d6000d14`  
		Last Modified: Wed, 27 May 2020 18:45:33 GMT  
		Size: 135.6 MB (135591772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7824f1fee1a2f0cd08b56fa89e23b0b6f638011b8c4ef4ea73459421a9e392d7`  
		Last Modified: Wed, 27 May 2020 18:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53634b129038dca0fdd69e092684760357550fe4e2af7a966bc58a6e2fa45bef`  
		Last Modified: Wed, 27 May 2020 18:45:43 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc-windowsservercore`

```console
$ docker pull mongo@sha256:d09845797e5bc2792e3ff4178eeb0604cd5d06bea5ef8e3aa7e1dee61492f7e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.4-rc-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:bd65d37f2b73020adb7e393b6de97b43f488263b8a0664fe2be5d43ffea318ce
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5782737930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0652785d046112fb8b7577d4309b99d566db1c54ecf7da51be1272fc8316c68e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 27 May 2020 18:14:44 GMT
ENV MONGO_VERSION=4.4.0-rc7
# Wed, 27 May 2020 18:14:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc7-signed.msi
# Wed, 27 May 2020 18:14:47 GMT
ENV MONGO_DOWNLOAD_SHA256=2cfcb05237b05c480761421a78126fcc69761e8396c99e222dcd433c0c5230f1
# Wed, 27 May 2020 18:30:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 27 May 2020 18:30:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 May 2020 18:30:37 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:30:38 GMT
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
	-	`sha256:b2152a451adb220520a5fca7a7f5ee9b59a5ee1c5890127e6d4e1513f1a6aeac`  
		Last Modified: Wed, 27 May 2020 18:51:01 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30527b5ff54f875584fc15d7ca1395fe3615b50fecc76b045bd19977f22f01c`  
		Last Modified: Wed, 27 May 2020 18:51:01 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702fa76eb41d5a6a00c325ada2aaf92a55fcda20232abaa2ccfb38cd0e6b64dd`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850bc1d85a1e940fec81fb23df0f146af25215abf892c9e4aa3920ee178a0240`  
		Last Modified: Wed, 27 May 2020 18:51:09 GMT  
		Size: 50.8 MB (50840027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0cd9a5e90d61da83a3ec185ff9c24055219e2d955317a8551521cf815bff57`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1243585b1cce5c1b0c05d2de35f71db8fbb19681b6fb1f64d6b0efdce529561f`  
		Last Modified: Wed, 27 May 2020 18:50:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f26a4c416d8d54aa9ad4186fed86dfe21d87ab19a8db9ed8659e0bc4841666e`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:70bc30df68902220e386532bf2337912d72b437f1974fec18458621f913acabb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2126230588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769dbe6ef1ce3d8d76060466c0feaa996319767448a3bf90a24e8aced08a75ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 27 May 2020 18:30:47 GMT
ENV MONGO_VERSION=4.4.0-rc7
# Wed, 27 May 2020 18:30:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc7-signed.msi
# Wed, 27 May 2020 18:30:48 GMT
ENV MONGO_DOWNLOAD_SHA256=2cfcb05237b05c480761421a78126fcc69761e8396c99e222dcd433c0c5230f1
# Wed, 27 May 2020 18:49:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 27 May 2020 18:49:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 May 2020 18:49:54 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:49:56 GMT
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
	-	`sha256:fb996e03af1eebd8fd548ac88e3ab9cb3d14b0b643573ca6c92ec319d98cabae`  
		Last Modified: Wed, 27 May 2020 18:51:21 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50dd2e8dc45ae9131283b60d78f26d56b824cf403cda9040c599900441bcfcb4`  
		Last Modified: Wed, 27 May 2020 18:51:21 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7feed001c9cff121f320362b36dc092d9043df9e5c725009867db7f0dcb4668`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e23083c29faa7ef259a9da86e2fc53d4cae2cfa3cf50cef3fdd392dfb5a097b`  
		Last Modified: Wed, 27 May 2020 18:52:15 GMT  
		Size: 407.9 MB (407889623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26005df8dc2749db3ea8a606283c1749ed8b1c49fb48f73e664eaba993663414`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb755abaacde5dc90adbaca2838324e3ae94dcc74f3819110d765b66e44506e8`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f69a4cd6bbf2a72ebb194850174a5672de9de41e8e8c33f1db1ef45445af9c7`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc-windowsservercore-1809`

```console
$ docker pull mongo@sha256:397e91683339f30823570df0116e84cbc5954bc0bf5f05203e8871c66235c3c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4.4-rc-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:70bc30df68902220e386532bf2337912d72b437f1974fec18458621f913acabb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2126230588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769dbe6ef1ce3d8d76060466c0feaa996319767448a3bf90a24e8aced08a75ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 27 May 2020 18:30:47 GMT
ENV MONGO_VERSION=4.4.0-rc7
# Wed, 27 May 2020 18:30:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc7-signed.msi
# Wed, 27 May 2020 18:30:48 GMT
ENV MONGO_DOWNLOAD_SHA256=2cfcb05237b05c480761421a78126fcc69761e8396c99e222dcd433c0c5230f1
# Wed, 27 May 2020 18:49:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 27 May 2020 18:49:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 May 2020 18:49:54 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:49:56 GMT
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
	-	`sha256:fb996e03af1eebd8fd548ac88e3ab9cb3d14b0b643573ca6c92ec319d98cabae`  
		Last Modified: Wed, 27 May 2020 18:51:21 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50dd2e8dc45ae9131283b60d78f26d56b824cf403cda9040c599900441bcfcb4`  
		Last Modified: Wed, 27 May 2020 18:51:21 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7feed001c9cff121f320362b36dc092d9043df9e5c725009867db7f0dcb4668`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e23083c29faa7ef259a9da86e2fc53d4cae2cfa3cf50cef3fdd392dfb5a097b`  
		Last Modified: Wed, 27 May 2020 18:52:15 GMT  
		Size: 407.9 MB (407889623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26005df8dc2749db3ea8a606283c1749ed8b1c49fb48f73e664eaba993663414`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb755abaacde5dc90adbaca2838324e3ae94dcc74f3819110d765b66e44506e8`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f69a4cd6bbf2a72ebb194850174a5672de9de41e8e8c33f1db1ef45445af9c7`  
		Last Modified: Wed, 27 May 2020 18:51:19 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:d3c8484189338a8223e194a5faa95e59db616769d5cdd4c7615bb35bd2ff1100
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4.4-rc-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:bd65d37f2b73020adb7e393b6de97b43f488263b8a0664fe2be5d43ffea318ce
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5782737930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0652785d046112fb8b7577d4309b99d566db1c54ecf7da51be1272fc8316c68e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 27 May 2020 18:14:44 GMT
ENV MONGO_VERSION=4.4.0-rc7
# Wed, 27 May 2020 18:14:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc7-signed.msi
# Wed, 27 May 2020 18:14:47 GMT
ENV MONGO_DOWNLOAD_SHA256=2cfcb05237b05c480761421a78126fcc69761e8396c99e222dcd433c0c5230f1
# Wed, 27 May 2020 18:30:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 27 May 2020 18:30:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 May 2020 18:30:37 GMT
EXPOSE 27017
# Wed, 27 May 2020 18:30:38 GMT
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
	-	`sha256:b2152a451adb220520a5fca7a7f5ee9b59a5ee1c5890127e6d4e1513f1a6aeac`  
		Last Modified: Wed, 27 May 2020 18:51:01 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30527b5ff54f875584fc15d7ca1395fe3615b50fecc76b045bd19977f22f01c`  
		Last Modified: Wed, 27 May 2020 18:51:01 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702fa76eb41d5a6a00c325ada2aaf92a55fcda20232abaa2ccfb38cd0e6b64dd`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850bc1d85a1e940fec81fb23df0f146af25215abf892c9e4aa3920ee178a0240`  
		Last Modified: Wed, 27 May 2020 18:51:09 GMT  
		Size: 50.8 MB (50840027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0cd9a5e90d61da83a3ec185ff9c24055219e2d955317a8551521cf815bff57`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1243585b1cce5c1b0c05d2de35f71db8fbb19681b6fb1f64d6b0efdce529561f`  
		Last Modified: Wed, 27 May 2020 18:50:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f26a4c416d8d54aa9ad4186fed86dfe21d87ab19a8db9ed8659e0bc4841666e`  
		Last Modified: Wed, 27 May 2020 18:50:58 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:9d5a8a478b36f9034b6b6ffca96e4172cacca8d2f0a0c96a5822bc01d518b116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:bd251a06b6423d0c37d37de1e19899b2d7b861df43d1b737b274cc95ac913885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164653603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68b650ad44f7a95c256ad2df5c40fbc3b13001f36ac7b7cd25f5f9a09be7d`
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
# Tue, 26 May 2020 22:37:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:37:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:37:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:37:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:37:52 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:37:53 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:37:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:37:53 GMT
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
	-	`sha256:978c572f04400f6e66309862a870a43ad987aadbb83dde6bf69aa704bd825175`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a600ffcf6a6cacd0d3e0eafddf0fa470759c45d3c11aebfb148c821f5ae66b`  
		Last Modified: Tue, 26 May 2020 22:40:51 GMT  
		Size: 129.1 MB (129113906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f812cdfe69fa174869fbf3ec347c097ac7db9f0ebe95263f818c27638c533`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8109e271104450b0ab84c81eb31ee3345711d7d41b35610029c44d15311dc9`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b8f41e6ed567bbb68d5cdb364664eef7c5f4f9bb628d25bb71fe1a532aea7856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154691636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580631906251de3ae7da70cd333fae9886d964e7e30d39e65b55c24a77093843`
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
# Tue, 26 May 2020 22:01:49 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:01:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:02:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:02:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:02:43 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:02:45 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:02:48 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:02:51 GMT
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
	-	`sha256:1ee6871420084682cb152ede4fb479d89174a0e623e68b93cfd21412586093b7`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23903f79dae06f8cc3aa422bb9893de8fcf91e92a504d05db484e34a0efbb91d`  
		Last Modified: Tue, 26 May 2020 22:03:45 GMT  
		Size: 122.9 MB (122905885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec235da2971da8b9af665d6caff32c9122bc5112a4c7280c57bd65f0283c2807`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac5d2db76761538d764cac5f29378ec6fdb214380caeb74730e620f2fbe529c`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:5d4da8f703443f19b3b0665a5e5922c5e349c2d2beaf88cd629db7faa0b3729f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160608601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a7890bfca6b2ee342feb02c588fd72bc4a84cf9c887a0d0647c9f92dcb4278`
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
# Tue, 26 May 2020 21:45:43 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 21:45:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 21:46:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 21:46:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 21:46:35 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 21:46:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 21:46:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 21:46:36 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:37 GMT
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
	-	`sha256:a211607bd79c344a64bd1823730cf4ff32c204005a9c31f6043d78322cfec773`  
		Last Modified: Tue, 26 May 2020 21:46:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358fcf8acc5b9c5439f270d6d7937fa6e3066ba8663568e4fcab9ce23fc7ffa7`  
		Last Modified: Tue, 26 May 2020 21:47:36 GMT  
		Size: 126.7 MB (126738794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba3c21f431df187bacc529912e2abec012ebc9d946e50ab3fed60a02bd3fbd`  
		Last Modified: Tue, 26 May 2020 21:47:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68d35b3abc69df8615e4bb3acec1fb6488e1c184b2c94d556cd5d47cc3fa46`  
		Last Modified: Tue, 26 May 2020 21:46:54 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:20055d57fb34769eeab26de814a41c9ecff2c0deff29ff9d523652ac2a0492dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:4-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0768e7755712a5a86421a0aad9801e3b4a46f639e89c231011e92a67bb1e59cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b465214c1a5519ea93ce8e61cf0a33f388b46c157984807f8e596a5665b75ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:9d5a8a478b36f9034b6b6ffca96e4172cacca8d2f0a0c96a5822bc01d518b116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:bd251a06b6423d0c37d37de1e19899b2d7b861df43d1b737b274cc95ac913885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164653603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68b650ad44f7a95c256ad2df5c40fbc3b13001f36ac7b7cd25f5f9a09be7d`
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
# Tue, 26 May 2020 22:37:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:37:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:37:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:37:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:37:52 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:37:53 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:37:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:37:53 GMT
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
	-	`sha256:978c572f04400f6e66309862a870a43ad987aadbb83dde6bf69aa704bd825175`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a600ffcf6a6cacd0d3e0eafddf0fa470759c45d3c11aebfb148c821f5ae66b`  
		Last Modified: Tue, 26 May 2020 22:40:51 GMT  
		Size: 129.1 MB (129113906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f812cdfe69fa174869fbf3ec347c097ac7db9f0ebe95263f818c27638c533`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8109e271104450b0ab84c81eb31ee3345711d7d41b35610029c44d15311dc9`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b8f41e6ed567bbb68d5cdb364664eef7c5f4f9bb628d25bb71fe1a532aea7856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154691636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580631906251de3ae7da70cd333fae9886d964e7e30d39e65b55c24a77093843`
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
# Tue, 26 May 2020 22:01:49 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:01:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:02:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:02:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:02:43 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:02:45 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:02:48 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:02:51 GMT
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
	-	`sha256:1ee6871420084682cb152ede4fb479d89174a0e623e68b93cfd21412586093b7`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23903f79dae06f8cc3aa422bb9893de8fcf91e92a504d05db484e34a0efbb91d`  
		Last Modified: Tue, 26 May 2020 22:03:45 GMT  
		Size: 122.9 MB (122905885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec235da2971da8b9af665d6caff32c9122bc5112a4c7280c57bd65f0283c2807`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac5d2db76761538d764cac5f29378ec6fdb214380caeb74730e620f2fbe529c`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:5d4da8f703443f19b3b0665a5e5922c5e349c2d2beaf88cd629db7faa0b3729f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160608601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a7890bfca6b2ee342feb02c588fd72bc4a84cf9c887a0d0647c9f92dcb4278`
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
# Tue, 26 May 2020 21:45:43 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 21:45:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 21:46:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 21:46:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 21:46:35 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 21:46:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 21:46:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 21:46:36 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:37 GMT
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
	-	`sha256:a211607bd79c344a64bd1823730cf4ff32c204005a9c31f6043d78322cfec773`  
		Last Modified: Tue, 26 May 2020 21:46:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358fcf8acc5b9c5439f270d6d7937fa6e3066ba8663568e4fcab9ce23fc7ffa7`  
		Last Modified: Tue, 26 May 2020 21:47:36 GMT  
		Size: 126.7 MB (126738794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba3c21f431df187bacc529912e2abec012ebc9d946e50ab3fed60a02bd3fbd`  
		Last Modified: Tue, 26 May 2020 21:47:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68d35b3abc69df8615e4bb3acec1fb6488e1c184b2c94d556cd5d47cc3fa46`  
		Last Modified: Tue, 26 May 2020 21:46:54 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:be8d903a68997dd63f64479004a7eeb4f0674dde7ab3cbd1145e5658da3a817b
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
$ docker pull mongo@sha256:bd251a06b6423d0c37d37de1e19899b2d7b861df43d1b737b274cc95ac913885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164653603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68b650ad44f7a95c256ad2df5c40fbc3b13001f36ac7b7cd25f5f9a09be7d`
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
# Tue, 26 May 2020 22:37:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:37:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:37:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:37:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:37:52 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:37:53 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:37:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:37:53 GMT
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
	-	`sha256:978c572f04400f6e66309862a870a43ad987aadbb83dde6bf69aa704bd825175`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a600ffcf6a6cacd0d3e0eafddf0fa470759c45d3c11aebfb148c821f5ae66b`  
		Last Modified: Tue, 26 May 2020 22:40:51 GMT  
		Size: 129.1 MB (129113906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f812cdfe69fa174869fbf3ec347c097ac7db9f0ebe95263f818c27638c533`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8109e271104450b0ab84c81eb31ee3345711d7d41b35610029c44d15311dc9`  
		Last Modified: Tue, 26 May 2020 22:38:06 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b8f41e6ed567bbb68d5cdb364664eef7c5f4f9bb628d25bb71fe1a532aea7856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154691636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580631906251de3ae7da70cd333fae9886d964e7e30d39e65b55c24a77093843`
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
# Tue, 26 May 2020 22:01:49 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:01:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 22:02:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 22:02:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 22:02:43 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 22:02:45 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 22:02:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 22:02:48 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:02:51 GMT
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
	-	`sha256:1ee6871420084682cb152ede4fb479d89174a0e623e68b93cfd21412586093b7`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23903f79dae06f8cc3aa422bb9893de8fcf91e92a504d05db484e34a0efbb91d`  
		Last Modified: Tue, 26 May 2020 22:03:45 GMT  
		Size: 122.9 MB (122905885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec235da2971da8b9af665d6caff32c9122bc5112a4c7280c57bd65f0283c2807`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac5d2db76761538d764cac5f29378ec6fdb214380caeb74730e620f2fbe529c`  
		Last Modified: Tue, 26 May 2020 22:03:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:5d4da8f703443f19b3b0665a5e5922c5e349c2d2beaf88cd629db7faa0b3729f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160608601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a7890bfca6b2ee342feb02c588fd72bc4a84cf9c887a0d0647c9f92dcb4278`
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
# Tue, 26 May 2020 21:45:43 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 21:45:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 26 May 2020 21:46:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 26 May 2020 21:46:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 26 May 2020 21:46:35 GMT
VOLUME [/data/db /data/configdb]
# Tue, 26 May 2020 21:46:35 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Tue, 26 May 2020 21:46:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 May 2020 21:46:36 GMT
EXPOSE 27017
# Tue, 26 May 2020 21:46:37 GMT
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
	-	`sha256:a211607bd79c344a64bd1823730cf4ff32c204005a9c31f6043d78322cfec773`  
		Last Modified: Tue, 26 May 2020 21:46:55 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358fcf8acc5b9c5439f270d6d7937fa6e3066ba8663568e4fcab9ce23fc7ffa7`  
		Last Modified: Tue, 26 May 2020 21:47:36 GMT  
		Size: 126.7 MB (126738794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba3c21f431df187bacc529912e2abec012ebc9d946e50ab3fed60a02bd3fbd`  
		Last Modified: Tue, 26 May 2020 21:47:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68d35b3abc69df8615e4bb3acec1fb6488e1c184b2c94d556cd5d47cc3fa46`  
		Last Modified: Tue, 26 May 2020 21:46:54 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:20055d57fb34769eeab26de814a41c9ecff2c0deff29ff9d523652ac2a0492dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:0768e7755712a5a86421a0aad9801e3b4a46f639e89c231011e92a67bb1e59cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:4ed9e722e7208713cd0db6a994342a5483148f86bc300bafd9f9f4e43bf42e86
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809830349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d954257223b8067b2f76ab42ca080fecccd675349304fb3dd346c6c2940500`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:44:00 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:44:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:44:02 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:59:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:59:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:59:53 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:59:54 GMT
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
	-	`sha256:148092c4435cf78eff436f984249c16455c3fd73ccd14fbd73a652c7d12c02ac`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a6670dd73092a916e2bb60d9cfd18576c62161e4d7378234d72762cc8390ea`  
		Last Modified: Tue, 26 May 2020 23:02:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbc9c56cf05c70234679ca9c4388698435cbc9048adc26a47462551f272e9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f012da451af8403018701ff858d9d57da34dfebf622dfdac58dd6e802852cbe6`  
		Last Modified: Tue, 26 May 2020 23:03:31 GMT  
		Size: 91.5 MB (91489428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b9807e649220503e2dd7f1cbee829c2dc204b226c8da31b7689673bcb5b6`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0994eba96cdc955f61635a7d34b69c2e2af2c075b0a80f08bc0844d57340b1`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0923e406427821d369de21bd06c7f171d01ec8c2d884cc08064b12c2c261dfe9`  
		Last Modified: Tue, 26 May 2020 23:02:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b465214c1a5519ea93ce8e61cf0a33f388b46c157984807f8e596a5665b75ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:f085fb326183128e5fe322894def5a10dda6318c7e2f74c1154c949d712da161
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6190835990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596b2a81f99a099b5cc99c2e9a3d55672efb2d6128350d64d2c4b4982d1bde`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 26 May 2020 22:25:26 GMT
ENV MONGO_VERSION=4.2.7
# Tue, 26 May 2020 22:25:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Tue, 26 May 2020 22:25:28 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Tue, 26 May 2020 22:43:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 26 May 2020 22:43:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 26 May 2020 22:43:47 GMT
EXPOSE 27017
# Tue, 26 May 2020 22:43:48 GMT
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
	-	`sha256:640e7a63c9aec24a469438efaa13fc121aaba0353301bc0c9ce413287c5150fb`  
		Last Modified: Tue, 26 May 2020 23:00:44 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bafbea768cc18739ff7e474820256298a49d05507183a84cdb810a21c76b4c`  
		Last Modified: Tue, 26 May 2020 23:00:43 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76418b70f7bbd1bb3a2a30f5565beb763a89566d6d01b14447e3f9ceba2e9a2f`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5be6494c2d31b3360315d66448589e34bbbddca7d7d38ca9efcf52e1e8916`  
		Last Modified: Tue, 26 May 2020 23:02:07 GMT  
		Size: 458.9 MB (458938127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ee012d50e96e3efb3f1b7446eeba4248b20c46dc6b74a313de76e4f06bb52`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf0b68ed52d45bba2dc25884be14ad40e6f686a4d3e8e0f21142aa4c131abc`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9edc3fe665f0e36f2337433e1aec7ab91290ed0c391725e2973a78a498eaac6`  
		Last Modified: Tue, 26 May 2020 23:00:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
