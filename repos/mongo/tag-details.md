<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.21`](#mongo3621)
-	[`mongo:3.6.21-windowsservercore`](#mongo3621-windowsservercore)
-	[`mongo:3.6.21-windowsservercore-1809`](#mongo3621-windowsservercore-1809)
-	[`mongo:3.6.21-windowsservercore-ltsc2016`](#mongo3621-windowsservercore-ltsc2016)
-	[`mongo:3.6.21-xenial`](#mongo3621-xenial)
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
-	[`mongo:4.0.22`](#mongo4022)
-	[`mongo:4.0.22-windowsservercore`](#mongo4022-windowsservercore)
-	[`mongo:4.0.22-windowsservercore-1809`](#mongo4022-windowsservercore-1809)
-	[`mongo:4.0.22-windowsservercore-ltsc2016`](#mongo4022-windowsservercore-ltsc2016)
-	[`mongo:4.0.22-xenial`](#mongo4022-xenial)
-	[`mongo:4.0-windowsservercore`](#mongo40-windowsservercore)
-	[`mongo:4.0-windowsservercore-1809`](#mongo40-windowsservercore-1809)
-	[`mongo:4.0-windowsservercore-ltsc2016`](#mongo40-windowsservercore-ltsc2016)
-	[`mongo:4.0-xenial`](#mongo40-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2.12`](#mongo4212)
-	[`mongo:4.2.12-bionic`](#mongo4212-bionic)
-	[`mongo:4.2.12-windowsservercore`](#mongo4212-windowsservercore)
-	[`mongo:4.2.12-windowsservercore-1809`](#mongo4212-windowsservercore-1809)
-	[`mongo:4.2.12-windowsservercore-ltsc2016`](#mongo4212-windowsservercore-ltsc2016)
-	[`mongo:4.2-bionic`](#mongo42-bionic)
-	[`mongo:4.2-windowsservercore`](#mongo42-windowsservercore)
-	[`mongo:4.2-windowsservercore-1809`](#mongo42-windowsservercore-1809)
-	[`mongo:4.2-windowsservercore-ltsc2016`](#mongo42-windowsservercore-ltsc2016)
-	[`mongo:4.4`](#mongo44)
-	[`mongo:4.4.3`](#mongo443)
-	[`mongo:4.4.3-bionic`](#mongo443-bionic)
-	[`mongo:4.4.3-windowsservercore`](#mongo443-windowsservercore)
-	[`mongo:4.4.3-windowsservercore-1809`](#mongo443-windowsservercore-1809)
-	[`mongo:4.4.3-windowsservercore-ltsc2016`](#mongo443-windowsservercore-ltsc2016)
-	[`mongo:4.4-bionic`](#mongo44-bionic)
-	[`mongo:4.4-windowsservercore`](#mongo44-windowsservercore)
-	[`mongo:4.4-windowsservercore-1809`](#mongo44-windowsservercore-1809)
-	[`mongo:4.4-windowsservercore-ltsc2016`](#mongo44-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:3cff2069adb34a330552695659c261bca69148e325863763b78b0285dd1a25c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:6e5d3405a510988d96f0fa3ec7220040be27ce783eb4cd576feb1a69b382ea20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168084432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff3e31881d4de60f682b930731fffb4b35dd76b575f9dd45a43792c16797ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:28 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 10:21:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 10:21:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:21:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:21:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:21:48 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:21:49 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:21:49 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:21:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fda94ce451d72c56874ac855ff0705d50e79d18529cafeb62f9fa58de95cf5`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b352c6b0992b87a33cd9eb0bc3cc7723f9c46da6e4d2c86fc21bacb87d072e00`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1fc6762a1396f2367d67a28c34fbf08a64a48cd692cf5e5fd636015bc0673`  
		Last Modified: Thu, 21 Jan 2021 10:24:47 GMT  
		Size: 117.9 MB (117885898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba02136cb0fe6eb1d97a3a8f2fcab2ced7859c7c6499886f24784f42d88e6d6f`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4005fc549570ef20efc0d68961844194b3de3f8b46425d5c1c9b535fc211b2`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8226c9734c19533d5cc52748e35ae10085f3b4ef0a3bd4537017bc2484589511
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156567673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77d2e2a70d8f0d9963398d15dcaee47e6da18633afdeb71b8e26c7c3f914da3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:51:54 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 05:51:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:51:57 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:51:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 05:52:01 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 05:52:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:52:26 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:52:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:52:30 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:52:30 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:52:32 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:52:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bdd40f932aa2d4c7c7c4c7caefe9424acf19474a68099912de7b7e65e8c9ca`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01594579b2917ebbf8d75bf5e04b7e3323d7628998ceb6caf71e19bb019ec37f`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e3e146ea59379808e302cccaffddee09bf024591db1f7a9bb354c80c2c9a3`  
		Last Modified: Thu, 21 Jan 2021 05:56:57 GMT  
		Size: 112.0 MB (111992049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee19bd675819baac4e15697f45116c97ca6920499a3d7f021e0627c38352c17`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a05bfdf189395ad97d4bee21218e828247af2171c960e7c5fff530c99dc332`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:3cff2069adb34a330552695659c261bca69148e325863763b78b0285dd1a25c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:6e5d3405a510988d96f0fa3ec7220040be27ce783eb4cd576feb1a69b382ea20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168084432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff3e31881d4de60f682b930731fffb4b35dd76b575f9dd45a43792c16797ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:28 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 10:21:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 10:21:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:21:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:21:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:21:48 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:21:49 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:21:49 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:21:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fda94ce451d72c56874ac855ff0705d50e79d18529cafeb62f9fa58de95cf5`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b352c6b0992b87a33cd9eb0bc3cc7723f9c46da6e4d2c86fc21bacb87d072e00`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1fc6762a1396f2367d67a28c34fbf08a64a48cd692cf5e5fd636015bc0673`  
		Last Modified: Thu, 21 Jan 2021 10:24:47 GMT  
		Size: 117.9 MB (117885898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba02136cb0fe6eb1d97a3a8f2fcab2ced7859c7c6499886f24784f42d88e6d6f`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4005fc549570ef20efc0d68961844194b3de3f8b46425d5c1c9b535fc211b2`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8226c9734c19533d5cc52748e35ae10085f3b4ef0a3bd4537017bc2484589511
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156567673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77d2e2a70d8f0d9963398d15dcaee47e6da18633afdeb71b8e26c7c3f914da3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:51:54 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 05:51:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:51:57 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:51:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 05:52:01 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 05:52:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:52:26 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:52:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:52:30 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:52:30 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:52:32 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:52:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bdd40f932aa2d4c7c7c4c7caefe9424acf19474a68099912de7b7e65e8c9ca`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01594579b2917ebbf8d75bf5e04b7e3323d7628998ceb6caf71e19bb019ec37f`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e3e146ea59379808e302cccaffddee09bf024591db1f7a9bb354c80c2c9a3`  
		Last Modified: Thu, 21 Jan 2021 05:56:57 GMT  
		Size: 112.0 MB (111992049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee19bd675819baac4e15697f45116c97ca6920499a3d7f021e0627c38352c17`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a05bfdf189395ad97d4bee21218e828247af2171c960e7c5fff530c99dc332`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21`

```console
$ docker pull mongo@sha256:3cff2069adb34a330552695659c261bca69148e325863763b78b0285dd1a25c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:3.6.21` - linux; amd64

```console
$ docker pull mongo@sha256:6e5d3405a510988d96f0fa3ec7220040be27ce783eb4cd576feb1a69b382ea20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168084432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff3e31881d4de60f682b930731fffb4b35dd76b575f9dd45a43792c16797ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:28 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 10:21:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 10:21:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:21:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:21:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:21:48 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:21:49 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:21:49 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:21:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fda94ce451d72c56874ac855ff0705d50e79d18529cafeb62f9fa58de95cf5`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b352c6b0992b87a33cd9eb0bc3cc7723f9c46da6e4d2c86fc21bacb87d072e00`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1fc6762a1396f2367d67a28c34fbf08a64a48cd692cf5e5fd636015bc0673`  
		Last Modified: Thu, 21 Jan 2021 10:24:47 GMT  
		Size: 117.9 MB (117885898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba02136cb0fe6eb1d97a3a8f2fcab2ced7859c7c6499886f24784f42d88e6d6f`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4005fc549570ef20efc0d68961844194b3de3f8b46425d5c1c9b535fc211b2`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8226c9734c19533d5cc52748e35ae10085f3b4ef0a3bd4537017bc2484589511
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156567673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77d2e2a70d8f0d9963398d15dcaee47e6da18633afdeb71b8e26c7c3f914da3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:51:54 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 05:51:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:51:57 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:51:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 05:52:01 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 05:52:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:52:26 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:52:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:52:30 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:52:30 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:52:32 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:52:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bdd40f932aa2d4c7c7c4c7caefe9424acf19474a68099912de7b7e65e8c9ca`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01594579b2917ebbf8d75bf5e04b7e3323d7628998ceb6caf71e19bb019ec37f`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e3e146ea59379808e302cccaffddee09bf024591db1f7a9bb354c80c2c9a3`  
		Last Modified: Thu, 21 Jan 2021 05:56:57 GMT  
		Size: 112.0 MB (111992049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee19bd675819baac4e15697f45116c97ca6920499a3d7f021e0627c38352c17`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a05bfdf189395ad97d4bee21218e828247af2171c960e7c5fff530c99dc332`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21-windowsservercore`

```console
$ docker pull mongo@sha256:e537c1be9d0c145e4db94b31116ab64708226c840eb13aad75e06bc800197a10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:3.6.21-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21-windowsservercore-1809`

```console
$ docker pull mongo@sha256:53d65024218b7ec470d28d5d223fe2cb132824d8263713f15ae60c55bfd53546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:3.6.21-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:13b11848469d499c0f47c7b7ba319025ecac7c638fc74193369fe6d35c7dae77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:3.6.21-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21-xenial`

```console
$ docker pull mongo@sha256:ad5bb61b0ae6c5172767186026a28e2580edb1de858dfa555943ee26518166a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.21-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:6e5d3405a510988d96f0fa3ec7220040be27ce783eb4cd576feb1a69b382ea20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168084432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff3e31881d4de60f682b930731fffb4b35dd76b575f9dd45a43792c16797ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:28 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 10:21:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 10:21:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:21:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:21:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:21:48 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:21:49 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:21:49 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:21:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fda94ce451d72c56874ac855ff0705d50e79d18529cafeb62f9fa58de95cf5`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b352c6b0992b87a33cd9eb0bc3cc7723f9c46da6e4d2c86fc21bacb87d072e00`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1fc6762a1396f2367d67a28c34fbf08a64a48cd692cf5e5fd636015bc0673`  
		Last Modified: Thu, 21 Jan 2021 10:24:47 GMT  
		Size: 117.9 MB (117885898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba02136cb0fe6eb1d97a3a8f2fcab2ced7859c7c6499886f24784f42d88e6d6f`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4005fc549570ef20efc0d68961844194b3de3f8b46425d5c1c9b535fc211b2`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8226c9734c19533d5cc52748e35ae10085f3b4ef0a3bd4537017bc2484589511
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156567673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77d2e2a70d8f0d9963398d15dcaee47e6da18633afdeb71b8e26c7c3f914da3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:51:54 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 05:51:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:51:57 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:51:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 05:52:01 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 05:52:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:52:26 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:52:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:52:30 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:52:30 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:52:32 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:52:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bdd40f932aa2d4c7c7c4c7caefe9424acf19474a68099912de7b7e65e8c9ca`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01594579b2917ebbf8d75bf5e04b7e3323d7628998ceb6caf71e19bb019ec37f`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e3e146ea59379808e302cccaffddee09bf024591db1f7a9bb354c80c2c9a3`  
		Last Modified: Thu, 21 Jan 2021 05:56:57 GMT  
		Size: 112.0 MB (111992049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee19bd675819baac4e15697f45116c97ca6920499a3d7f021e0627c38352c17`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a05bfdf189395ad97d4bee21218e828247af2171c960e7c5fff530c99dc332`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:e537c1be9d0c145e4db94b31116ab64708226c840eb13aad75e06bc800197a10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:53d65024218b7ec470d28d5d223fe2cb132824d8263713f15ae60c55bfd53546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:13b11848469d499c0f47c7b7ba319025ecac7c638fc74193369fe6d35c7dae77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:ad5bb61b0ae6c5172767186026a28e2580edb1de858dfa555943ee26518166a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:6e5d3405a510988d96f0fa3ec7220040be27ce783eb4cd576feb1a69b382ea20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168084432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff3e31881d4de60f682b930731fffb4b35dd76b575f9dd45a43792c16797ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:28 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 10:21:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 10:21:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:21:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:21:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:21:48 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:21:49 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:21:49 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:21:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fda94ce451d72c56874ac855ff0705d50e79d18529cafeb62f9fa58de95cf5`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b352c6b0992b87a33cd9eb0bc3cc7723f9c46da6e4d2c86fc21bacb87d072e00`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1fc6762a1396f2367d67a28c34fbf08a64a48cd692cf5e5fd636015bc0673`  
		Last Modified: Thu, 21 Jan 2021 10:24:47 GMT  
		Size: 117.9 MB (117885898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba02136cb0fe6eb1d97a3a8f2fcab2ced7859c7c6499886f24784f42d88e6d6f`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4005fc549570ef20efc0d68961844194b3de3f8b46425d5c1c9b535fc211b2`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8226c9734c19533d5cc52748e35ae10085f3b4ef0a3bd4537017bc2484589511
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156567673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77d2e2a70d8f0d9963398d15dcaee47e6da18633afdeb71b8e26c7c3f914da3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:51:54 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 05:51:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:51:57 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:51:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 05:52:01 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 05:52:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:52:26 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:52:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:52:30 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:52:30 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:52:32 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:52:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bdd40f932aa2d4c7c7c4c7caefe9424acf19474a68099912de7b7e65e8c9ca`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01594579b2917ebbf8d75bf5e04b7e3323d7628998ceb6caf71e19bb019ec37f`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e3e146ea59379808e302cccaffddee09bf024591db1f7a9bb354c80c2c9a3`  
		Last Modified: Thu, 21 Jan 2021 05:56:57 GMT  
		Size: 112.0 MB (111992049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee19bd675819baac4e15697f45116c97ca6920499a3d7f021e0627c38352c17`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a05bfdf189395ad97d4bee21218e828247af2171c960e7c5fff530c99dc332`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:e537c1be9d0c145e4db94b31116ab64708226c840eb13aad75e06bc800197a10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:3-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:53d65024218b7ec470d28d5d223fe2cb132824d8263713f15ae60c55bfd53546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fb9e9376b228ba8d75d62b10aadaa3ed445266f85e27af3da531666d992f9621
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2664861593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021b06d5154ebe72a4c643834d7b79914bf89bda74f8969de12a9247e6ecf9ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:23:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:23:10 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:26:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:26:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:26:32 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:26:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca50f45c0dd76e7202bbd60168c99c203e4bb6441c44a7cc9da9587df764aee`  
		Last Modified: Thu, 14 Jan 2021 00:57:32 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aba66b27badd60988ea21849d80f19e3f28b4080ffd73805391ca19c5bf778`  
		Last Modified: Thu, 14 Jan 2021 00:57:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85149e414b449654dd5b08293f608a73339af0c086a53ae28e3ec4ee296993`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4117320dac41affb2064d4240581dffafef75e7410a142e5e77e8afe47d36e`  
		Last Modified: Thu, 14 Jan 2021 00:58:15 GMT  
		Size: 229.1 MB (229081542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75afd4919400223446e1015339379353adf3f813ea3c0ae8f68c6d7e552558`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b7f817577d9539c1162a17c17eb4eebacbda2a6663cb25441975af618cec8a`  
		Last Modified: Thu, 14 Jan 2021 00:57:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada28003068dbc8c3ca86d83fc6da89b2b8b5c332684bbeeeb7f2dd7cdda6649`  
		Last Modified: Thu, 14 Jan 2021 00:57:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:13b11848469d499c0f47c7b7ba319025ecac7c638fc74193369fe6d35c7dae77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:ad5bb61b0ae6c5172767186026a28e2580edb1de858dfa555943ee26518166a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:6e5d3405a510988d96f0fa3ec7220040be27ce783eb4cd576feb1a69b382ea20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168084432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff3e31881d4de60f682b930731fffb4b35dd76b575f9dd45a43792c16797ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:28 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 10:21:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:21:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 10:21:30 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 10:21:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:21:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:21:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:21:48 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:21:49 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:21:49 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:21:49 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fda94ce451d72c56874ac855ff0705d50e79d18529cafeb62f9fa58de95cf5`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b352c6b0992b87a33cd9eb0bc3cc7723f9c46da6e4d2c86fc21bacb87d072e00`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1fc6762a1396f2367d67a28c34fbf08a64a48cd692cf5e5fd636015bc0673`  
		Last Modified: Thu, 21 Jan 2021 10:24:47 GMT  
		Size: 117.9 MB (117885898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba02136cb0fe6eb1d97a3a8f2fcab2ced7859c7c6499886f24784f42d88e6d6f`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4005fc549570ef20efc0d68961844194b3de3f8b46425d5c1c9b535fc211b2`  
		Last Modified: Thu, 21 Jan 2021 10:24:28 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8226c9734c19533d5cc52748e35ae10085f3b4ef0a3bd4537017bc2484589511
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156567673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77d2e2a70d8f0d9963398d15dcaee47e6da18633afdeb71b8e26c7c3f914da3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:51:54 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Jan 2021 05:51:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:51:57 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:51:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:00 GMT
ENV MONGO_MAJOR=3.6
# Thu, 21 Jan 2021 05:52:01 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 21 Jan 2021 05:52:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:52:26 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:52:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:52:30 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:52:30 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:52:32 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:52:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bdd40f932aa2d4c7c7c4c7caefe9424acf19474a68099912de7b7e65e8c9ca`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01594579b2917ebbf8d75bf5e04b7e3323d7628998ceb6caf71e19bb019ec37f`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e3e146ea59379808e302cccaffddee09bf024591db1f7a9bb354c80c2c9a3`  
		Last Modified: Thu, 21 Jan 2021 05:56:57 GMT  
		Size: 112.0 MB (111992049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee19bd675819baac4e15697f45116c97ca6920499a3d7f021e0627c38352c17`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a05bfdf189395ad97d4bee21218e828247af2171c960e7c5fff530c99dc332`  
		Last Modified: Thu, 21 Jan 2021 05:56:33 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:88e0308671a06d4ee7da41f87944ba66355b4ee3d57d57caf92f5e1938736abd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:06ba42906e0346c15a795ff6ebcb3ac88be0f85aa899a6225979029188e312c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178222610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8e14b1fda68aedb435fec2a6eaa326cf5633fc57b7e28b5cc37d938ead9edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:23:24 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 10:23:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:26 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 10:23:28 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:52 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:52 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca70046d298d7aac215eecead78d18f8f28e11eaea6db7f35c945e64a43124`  
		Last Modified: Thu, 21 Jan 2021 10:25:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a541da2a89089f196a998312c16f37f8ee11251f88d764ce95274dd29d5a3`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18edd0c32639b9f81da45ecc082e23f67c7eb02bc3a1216622dfe181c852f505`  
		Last Modified: Thu, 21 Jan 2021 10:26:20 GMT  
		Size: 142.7 MB (142686014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86830e28cf719e7b6459badd7a5ade676e32d9b08c004774f65dce25bc639636`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1d772417d960c2608d622279c356232f0b70a0b82c7129bf57df7f4c1aeea`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:35d866a5fd70ff9b9cd520ad48bc4250f1a4e05171b205fcfc68fe9c51efa8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168151561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095aea9826c2c421ae2b1c4299766ba6461174f3a901019cb427b1d1cf54f5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:55:16 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 05:55:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:55:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:55:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:21 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 05:55:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:55:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:55:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:55:55 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:55:56 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:57 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:55:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f46ba3c06d737a4d0e64c1f3db503400ee0eb1b4b4bb586b0bd7f9ded60c3a`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144bd8644f0fbdd12fa8e9850c9036f763fb7720a1a580a0ad88bd9c35fc4684`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250692aff7a7255ff3544fd94c39f0a2896636ced434869481c1029047068c4`  
		Last Modified: Thu, 21 Jan 2021 05:58:51 GMT  
		Size: 136.4 MB (136380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f467e359b3608c8a4425b25553555612e50e64f8e954c382195fcf3cd28401d0`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a524c0aa3acb289bb84a7514ddf6c6ac6cb5feb52a04d253aedc50de4a73488e`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:9c0b379fa79bc55520a9badaf4ac04a213d55e2e76c1f453261e7010e62c1b82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173132528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc71b87dda565765e825ef3f366cd24b6512c3c1495ee26e640d82412d9ed5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 04:00:45 GMT
ADD file:d443bbf06b974365e3cb2d99eea08d454059cf95b82a6023e4260fba5ead568e in / 
# Thu, 21 Jan 2021 04:00:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:00:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:00:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:00:56 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 04:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:39:49 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 04:39:50 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 04:40:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 04:40:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 04:40:15 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 04:40:17 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 04:40:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 04:41:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 04:41:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 04:41:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 04:41:25 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 04:41:27 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 04:41:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1a4e1c3f599543fe1043f321c3c5e14f5ca6073cba211f2144b569c5d0cff014`  
		Last Modified: Thu, 21 Jan 2021 04:03:17 GMT  
		Size: 25.4 MB (25381801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1202f2791a7390dbd7197d4cfde724e184be1b2f9d4791890fb64341336f889e`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c44bad24828f92a8ff703d4d356f2969f0c1de9f6d852d3cec338a3aff6265`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad237e33328657490128a3945e880b746ebd50c75cc14cb7e6cb1e2c60e8a1b`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2023f0f19357e97e77398f90b92a5736e2f71e3413a2fdc91330fc05461250`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 2.7 MB (2721180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb06349457fa157b55404be7a301c14dce1915009bad7fa29e12925d5821993`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 5.7 MB (5746846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33428088ab5395067d4b3d3b8dee47ab7f7237cdd0a4df0e3f6b8521c3fb839b`  
		Last Modified: Thu, 21 Jan 2021 04:42:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3464b0455ffb640246507864b1476076c6d50b7235fbc64c3bfd8e5660f4537`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684dd6070aa89f7d64e27f891d77a5fea632b893241ff66da06f16e54b3c96a6`  
		Last Modified: Thu, 21 Jan 2021 04:42:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c67edb3d568d86357a630edc1923d8fa70e3eea8bc5920edcf29dab66f11d4`  
		Last Modified: Thu, 21 Jan 2021 04:42:22 GMT  
		Size: 139.3 MB (139273378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e1ffd4eb011cb4d1416bf7f49751b13a4dfb5b0c37238e672290617b87dcf4`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efad1d47d721328a8ba57a39bc62b6560d33378f004345c4e3b5c39baf6fd48`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:fafd7c6063fd7f67bff7587182c8f5322232eca719c04f4b3da2ffc05ccc85ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:d6b5eecd9cc3058e4fb96231d67fb6bebd1cf3ac6f1fb8d0a60b1428872a57b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156112747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5323653a57085662bb404d44b61b663c3ad7485b4b04cfcdf8142215d14df946`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 21 Jan 2021 10:22:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:22:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:22:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:01 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:01 GMT
ENV MONGO_MAJOR=4.0
# Thu, 21 Jan 2021 10:22:02 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 21 Jan 2021 10:22:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:22:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:22:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:22:21 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:22:21 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:22:22 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:22:22 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4269ba38e222385bbc1282954ab869eb75e0e5bb3c1a29b8ad099c1d9ff1b39c`  
		Last Modified: Thu, 21 Jan 2021 10:24:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09264a562b57502b707476cea86b9deda6c6317b2e6cb33ccfedf68c801dc973`  
		Last Modified: Thu, 21 Jan 2021 10:24:58 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6bda190fde0bcecd34358c67051c874ffcd7a879b0b1ca9f10c4d1ef7590d`  
		Last Modified: Thu, 21 Jan 2021 10:25:19 GMT  
		Size: 105.9 MB (105914783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feafd2669d078147527d8449eb8c5e67d0440d398880bb621b5984d107d70967`  
		Last Modified: Thu, 21 Jan 2021 10:24:56 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b490a7d89210b3938d48f47fc8e24c055521a3698fbd88d96902b7e100a709`  
		Last Modified: Thu, 21 Jan 2021 10:24:56 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:89ca5fc8233cacf64b807339363dae970e66431153d33c5aed085dd517d71780
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144864314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0877e91206551ce59ec4e3a7223fc27e5fbb751d438d6f681b10a467083e945b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:52:45 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 21 Jan 2021 05:52:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:52:47 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:52:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:49 GMT
ENV MONGO_MAJOR=4.0
# Thu, 21 Jan 2021 05:52:50 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 21 Jan 2021 05:52:51 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:53:23 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:53:26 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:53:26 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:53:27 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:53:28 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:53:29 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b0c8486feab611ac6970c3c8b66319e41a420989534cef3ee891dc82d0c66d`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208ae58d870775a30f78775d29b6eca77bd4596309b196231d41d0f6d00a1df`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cd462b9c75d9dc145a81e4fed8cbf5cd29c1a12c720b4ea213b4612f934b7`  
		Last Modified: Thu, 21 Jan 2021 05:57:30 GMT  
		Size: 100.3 MB (100289261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4cc58789aa6a6c634b35d002d0fe11838513f31b45fa3bb1ce3cdd2e846a0a`  
		Last Modified: Thu, 21 Jan 2021 05:57:09 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed5f0a81ca68f0368b7f76dfae5c8fc7b58d7dc990c704226fc3aa27d7129d8`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:3d52f3757af0a7f9da0ead5abafb6b36d2f42c5ebe0a744c9f59fc9687103295
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2670616546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e6d7d88184b5b2147925eea1a075221df38e6aeb4c6ba52a0fc748ae4a25cf0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:31:03 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:34:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:34:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:34:33 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:34:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322c98bdb14c28d0b5869f41698820d62eabf2e257800da6fa66ff4f17606f23`  
		Last Modified: Thu, 14 Jan 2021 00:59:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e48c6d94fb782acb7b4dc1290faf8c878269b15b9e16293486a5638263c2d8`  
		Last Modified: Thu, 14 Jan 2021 00:59:47 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b0783fa10e8c1d7e4f627b97660f72c5c4f9949ebecfd58af8b34176f79009`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7a8d9c6e1146c13c0f64c47a9fdbd92c2802d228f842c64ff95e7ee67c0a8`  
		Last Modified: Thu, 14 Jan 2021 01:04:16 GMT  
		Size: 234.8 MB (234836390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1863d635dc8311d270ec8a6e3b7ece81eb4357cedbc7160fe58826002f181872`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118baad55a6f99b1acf8a65f36f502a179af8657666d6fd3a782db7266cb561`  
		Last Modified: Thu, 14 Jan 2021 00:59:46 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1f370df1c211a9cadb44a5fd531f53bf58e480df62d0f7acd7c348b578963`  
		Last Modified: Thu, 14 Jan 2021 00:59:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:1b9e1c2cc2e5cca86c706bd706f20568943ad81f6cc427636fcbcf5a8cf7ee9e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6029479083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1969addeb88f3b28d316a642745777fb088614191093025a93670be55d11b1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:34:45 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:38:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:38:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:38:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:39:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268fad4c2c60d1a5eee3ffa02942be8417db10862183c4a8de139ce38d76b42f`  
		Last Modified: Thu, 14 Jan 2021 01:04:47 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574240b920d1e70836565b0cb8167d0025f514dd9068a69974d5d2b258de4d`  
		Last Modified: Thu, 14 Jan 2021 01:04:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704f5df313ebfbb316d9e294be996801c1e4c2ae4da0446e1c3160134bf5cc50`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10bff8dc22cd39d534926404ce75b9a04689d9c9bdfafb6861111cc0972fea8`  
		Last Modified: Thu, 14 Jan 2021 01:08:55 GMT  
		Size: 235.6 MB (235577098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d49ac5bfb0015308d470e3638d64230ec947466b7d2e9e2ca0b5ce64c371b6`  
		Last Modified: Thu, 14 Jan 2021 01:04:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd6e1ff01caf85c900bcf6f7c979b463586791d084c6cb67773ffed35135357`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b66fee24b0f0b4659dc51e91583c75c7e80f7ffa051e2ec710808d07f844d`  
		Last Modified: Thu, 14 Jan 2021 01:04:42 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22`

```console
$ docker pull mongo@sha256:fafd7c6063fd7f67bff7587182c8f5322232eca719c04f4b3da2ffc05ccc85ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.0.22` - linux; amd64

```console
$ docker pull mongo@sha256:d6b5eecd9cc3058e4fb96231d67fb6bebd1cf3ac6f1fb8d0a60b1428872a57b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156112747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5323653a57085662bb404d44b61b663c3ad7485b4b04cfcdf8142215d14df946`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 21 Jan 2021 10:22:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:22:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:22:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:01 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:01 GMT
ENV MONGO_MAJOR=4.0
# Thu, 21 Jan 2021 10:22:02 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 21 Jan 2021 10:22:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:22:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:22:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:22:21 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:22:21 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:22:22 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:22:22 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4269ba38e222385bbc1282954ab869eb75e0e5bb3c1a29b8ad099c1d9ff1b39c`  
		Last Modified: Thu, 21 Jan 2021 10:24:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09264a562b57502b707476cea86b9deda6c6317b2e6cb33ccfedf68c801dc973`  
		Last Modified: Thu, 21 Jan 2021 10:24:58 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6bda190fde0bcecd34358c67051c874ffcd7a879b0b1ca9f10c4d1ef7590d`  
		Last Modified: Thu, 21 Jan 2021 10:25:19 GMT  
		Size: 105.9 MB (105914783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feafd2669d078147527d8449eb8c5e67d0440d398880bb621b5984d107d70967`  
		Last Modified: Thu, 21 Jan 2021 10:24:56 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b490a7d89210b3938d48f47fc8e24c055521a3698fbd88d96902b7e100a709`  
		Last Modified: Thu, 21 Jan 2021 10:24:56 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:89ca5fc8233cacf64b807339363dae970e66431153d33c5aed085dd517d71780
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144864314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0877e91206551ce59ec4e3a7223fc27e5fbb751d438d6f681b10a467083e945b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:52:45 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 21 Jan 2021 05:52:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:52:47 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:52:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:49 GMT
ENV MONGO_MAJOR=4.0
# Thu, 21 Jan 2021 05:52:50 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 21 Jan 2021 05:52:51 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:53:23 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:53:26 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:53:26 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:53:27 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:53:28 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:53:29 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b0c8486feab611ac6970c3c8b66319e41a420989534cef3ee891dc82d0c66d`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208ae58d870775a30f78775d29b6eca77bd4596309b196231d41d0f6d00a1df`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cd462b9c75d9dc145a81e4fed8cbf5cd29c1a12c720b4ea213b4612f934b7`  
		Last Modified: Thu, 21 Jan 2021 05:57:30 GMT  
		Size: 100.3 MB (100289261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4cc58789aa6a6c634b35d002d0fe11838513f31b45fa3bb1ce3cdd2e846a0a`  
		Last Modified: Thu, 21 Jan 2021 05:57:09 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed5f0a81ca68f0368b7f76dfae5c8fc7b58d7dc990c704226fc3aa27d7129d8`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:3d52f3757af0a7f9da0ead5abafb6b36d2f42c5ebe0a744c9f59fc9687103295
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2670616546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e6d7d88184b5b2147925eea1a075221df38e6aeb4c6ba52a0fc748ae4a25cf0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:31:03 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:34:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:34:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:34:33 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:34:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322c98bdb14c28d0b5869f41698820d62eabf2e257800da6fa66ff4f17606f23`  
		Last Modified: Thu, 14 Jan 2021 00:59:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e48c6d94fb782acb7b4dc1290faf8c878269b15b9e16293486a5638263c2d8`  
		Last Modified: Thu, 14 Jan 2021 00:59:47 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b0783fa10e8c1d7e4f627b97660f72c5c4f9949ebecfd58af8b34176f79009`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7a8d9c6e1146c13c0f64c47a9fdbd92c2802d228f842c64ff95e7ee67c0a8`  
		Last Modified: Thu, 14 Jan 2021 01:04:16 GMT  
		Size: 234.8 MB (234836390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1863d635dc8311d270ec8a6e3b7ece81eb4357cedbc7160fe58826002f181872`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118baad55a6f99b1acf8a65f36f502a179af8657666d6fd3a782db7266cb561`  
		Last Modified: Thu, 14 Jan 2021 00:59:46 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1f370df1c211a9cadb44a5fd531f53bf58e480df62d0f7acd7c348b578963`  
		Last Modified: Thu, 14 Jan 2021 00:59:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:1b9e1c2cc2e5cca86c706bd706f20568943ad81f6cc427636fcbcf5a8cf7ee9e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6029479083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1969addeb88f3b28d316a642745777fb088614191093025a93670be55d11b1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:34:45 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:38:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:38:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:38:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:39:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268fad4c2c60d1a5eee3ffa02942be8417db10862183c4a8de139ce38d76b42f`  
		Last Modified: Thu, 14 Jan 2021 01:04:47 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574240b920d1e70836565b0cb8167d0025f514dd9068a69974d5d2b258de4d`  
		Last Modified: Thu, 14 Jan 2021 01:04:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704f5df313ebfbb316d9e294be996801c1e4c2ae4da0446e1c3160134bf5cc50`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10bff8dc22cd39d534926404ce75b9a04689d9c9bdfafb6861111cc0972fea8`  
		Last Modified: Thu, 14 Jan 2021 01:08:55 GMT  
		Size: 235.6 MB (235577098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d49ac5bfb0015308d470e3638d64230ec947466b7d2e9e2ca0b5ce64c371b6`  
		Last Modified: Thu, 14 Jan 2021 01:04:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd6e1ff01caf85c900bcf6f7c979b463586791d084c6cb67773ffed35135357`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b66fee24b0f0b4659dc51e91583c75c7e80f7ffa051e2ec710808d07f844d`  
		Last Modified: Thu, 14 Jan 2021 01:04:42 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22-windowsservercore`

```console
$ docker pull mongo@sha256:487196e66d92bb3d1db5817a5d3a18b31b9b006e820c109692bbb22916841f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.0.22-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:3d52f3757af0a7f9da0ead5abafb6b36d2f42c5ebe0a744c9f59fc9687103295
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2670616546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e6d7d88184b5b2147925eea1a075221df38e6aeb4c6ba52a0fc748ae4a25cf0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:31:03 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:34:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:34:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:34:33 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:34:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322c98bdb14c28d0b5869f41698820d62eabf2e257800da6fa66ff4f17606f23`  
		Last Modified: Thu, 14 Jan 2021 00:59:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e48c6d94fb782acb7b4dc1290faf8c878269b15b9e16293486a5638263c2d8`  
		Last Modified: Thu, 14 Jan 2021 00:59:47 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b0783fa10e8c1d7e4f627b97660f72c5c4f9949ebecfd58af8b34176f79009`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7a8d9c6e1146c13c0f64c47a9fdbd92c2802d228f842c64ff95e7ee67c0a8`  
		Last Modified: Thu, 14 Jan 2021 01:04:16 GMT  
		Size: 234.8 MB (234836390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1863d635dc8311d270ec8a6e3b7ece81eb4357cedbc7160fe58826002f181872`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118baad55a6f99b1acf8a65f36f502a179af8657666d6fd3a782db7266cb561`  
		Last Modified: Thu, 14 Jan 2021 00:59:46 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1f370df1c211a9cadb44a5fd531f53bf58e480df62d0f7acd7c348b578963`  
		Last Modified: Thu, 14 Jan 2021 00:59:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:1b9e1c2cc2e5cca86c706bd706f20568943ad81f6cc427636fcbcf5a8cf7ee9e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6029479083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1969addeb88f3b28d316a642745777fb088614191093025a93670be55d11b1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:34:45 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:38:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:38:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:38:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:39:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268fad4c2c60d1a5eee3ffa02942be8417db10862183c4a8de139ce38d76b42f`  
		Last Modified: Thu, 14 Jan 2021 01:04:47 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574240b920d1e70836565b0cb8167d0025f514dd9068a69974d5d2b258de4d`  
		Last Modified: Thu, 14 Jan 2021 01:04:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704f5df313ebfbb316d9e294be996801c1e4c2ae4da0446e1c3160134bf5cc50`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10bff8dc22cd39d534926404ce75b9a04689d9c9bdfafb6861111cc0972fea8`  
		Last Modified: Thu, 14 Jan 2021 01:08:55 GMT  
		Size: 235.6 MB (235577098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d49ac5bfb0015308d470e3638d64230ec947466b7d2e9e2ca0b5ce64c371b6`  
		Last Modified: Thu, 14 Jan 2021 01:04:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd6e1ff01caf85c900bcf6f7c979b463586791d084c6cb67773ffed35135357`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b66fee24b0f0b4659dc51e91583c75c7e80f7ffa051e2ec710808d07f844d`  
		Last Modified: Thu, 14 Jan 2021 01:04:42 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0fbf918baaba9f3cec5268c6d37531bdf32471c9a58cbdfb61527fe8fbbaa07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:4.0.22-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:3d52f3757af0a7f9da0ead5abafb6b36d2f42c5ebe0a744c9f59fc9687103295
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2670616546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e6d7d88184b5b2147925eea1a075221df38e6aeb4c6ba52a0fc748ae4a25cf0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:31:03 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:34:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:34:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:34:33 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:34:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322c98bdb14c28d0b5869f41698820d62eabf2e257800da6fa66ff4f17606f23`  
		Last Modified: Thu, 14 Jan 2021 00:59:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e48c6d94fb782acb7b4dc1290faf8c878269b15b9e16293486a5638263c2d8`  
		Last Modified: Thu, 14 Jan 2021 00:59:47 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b0783fa10e8c1d7e4f627b97660f72c5c4f9949ebecfd58af8b34176f79009`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7a8d9c6e1146c13c0f64c47a9fdbd92c2802d228f842c64ff95e7ee67c0a8`  
		Last Modified: Thu, 14 Jan 2021 01:04:16 GMT  
		Size: 234.8 MB (234836390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1863d635dc8311d270ec8a6e3b7ece81eb4357cedbc7160fe58826002f181872`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118baad55a6f99b1acf8a65f36f502a179af8657666d6fd3a782db7266cb561`  
		Last Modified: Thu, 14 Jan 2021 00:59:46 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1f370df1c211a9cadb44a5fd531f53bf58e480df62d0f7acd7c348b578963`  
		Last Modified: Thu, 14 Jan 2021 00:59:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:4631ed2bd0f02e99bf90bc7434db1699f5717c319e384a3c5f964026c2416768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.0.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:1b9e1c2cc2e5cca86c706bd706f20568943ad81f6cc427636fcbcf5a8cf7ee9e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6029479083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1969addeb88f3b28d316a642745777fb088614191093025a93670be55d11b1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:34:45 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:38:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:38:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:38:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:39:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268fad4c2c60d1a5eee3ffa02942be8417db10862183c4a8de139ce38d76b42f`  
		Last Modified: Thu, 14 Jan 2021 01:04:47 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574240b920d1e70836565b0cb8167d0025f514dd9068a69974d5d2b258de4d`  
		Last Modified: Thu, 14 Jan 2021 01:04:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704f5df313ebfbb316d9e294be996801c1e4c2ae4da0446e1c3160134bf5cc50`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10bff8dc22cd39d534926404ce75b9a04689d9c9bdfafb6861111cc0972fea8`  
		Last Modified: Thu, 14 Jan 2021 01:08:55 GMT  
		Size: 235.6 MB (235577098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d49ac5bfb0015308d470e3638d64230ec947466b7d2e9e2ca0b5ce64c371b6`  
		Last Modified: Thu, 14 Jan 2021 01:04:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd6e1ff01caf85c900bcf6f7c979b463586791d084c6cb67773ffed35135357`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b66fee24b0f0b4659dc51e91583c75c7e80f7ffa051e2ec710808d07f844d`  
		Last Modified: Thu, 14 Jan 2021 01:04:42 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22-xenial`

```console
$ docker pull mongo@sha256:1ea6e4fb08cc9f00b89d3db37a64256266018d252fdbe2b319587cfa18d6ccfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.22-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:d6b5eecd9cc3058e4fb96231d67fb6bebd1cf3ac6f1fb8d0a60b1428872a57b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156112747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5323653a57085662bb404d44b61b663c3ad7485b4b04cfcdf8142215d14df946`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 21 Jan 2021 10:22:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:22:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:22:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:01 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:01 GMT
ENV MONGO_MAJOR=4.0
# Thu, 21 Jan 2021 10:22:02 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 21 Jan 2021 10:22:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:22:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:22:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:22:21 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:22:21 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:22:22 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:22:22 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4269ba38e222385bbc1282954ab869eb75e0e5bb3c1a29b8ad099c1d9ff1b39c`  
		Last Modified: Thu, 21 Jan 2021 10:24:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09264a562b57502b707476cea86b9deda6c6317b2e6cb33ccfedf68c801dc973`  
		Last Modified: Thu, 21 Jan 2021 10:24:58 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6bda190fde0bcecd34358c67051c874ffcd7a879b0b1ca9f10c4d1ef7590d`  
		Last Modified: Thu, 21 Jan 2021 10:25:19 GMT  
		Size: 105.9 MB (105914783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feafd2669d078147527d8449eb8c5e67d0440d398880bb621b5984d107d70967`  
		Last Modified: Thu, 21 Jan 2021 10:24:56 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b490a7d89210b3938d48f47fc8e24c055521a3698fbd88d96902b7e100a709`  
		Last Modified: Thu, 21 Jan 2021 10:24:56 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:89ca5fc8233cacf64b807339363dae970e66431153d33c5aed085dd517d71780
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144864314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0877e91206551ce59ec4e3a7223fc27e5fbb751d438d6f681b10a467083e945b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:52:45 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 21 Jan 2021 05:52:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:52:47 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:52:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:49 GMT
ENV MONGO_MAJOR=4.0
# Thu, 21 Jan 2021 05:52:50 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 21 Jan 2021 05:52:51 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:53:23 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:53:26 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:53:26 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:53:27 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:53:28 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:53:29 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b0c8486feab611ac6970c3c8b66319e41a420989534cef3ee891dc82d0c66d`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208ae58d870775a30f78775d29b6eca77bd4596309b196231d41d0f6d00a1df`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cd462b9c75d9dc145a81e4fed8cbf5cd29c1a12c720b4ea213b4612f934b7`  
		Last Modified: Thu, 21 Jan 2021 05:57:30 GMT  
		Size: 100.3 MB (100289261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4cc58789aa6a6c634b35d002d0fe11838513f31b45fa3bb1ce3cdd2e846a0a`  
		Last Modified: Thu, 21 Jan 2021 05:57:09 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed5f0a81ca68f0368b7f76dfae5c8fc7b58d7dc990c704226fc3aa27d7129d8`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:487196e66d92bb3d1db5817a5d3a18b31b9b006e820c109692bbb22916841f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:3d52f3757af0a7f9da0ead5abafb6b36d2f42c5ebe0a744c9f59fc9687103295
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2670616546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e6d7d88184b5b2147925eea1a075221df38e6aeb4c6ba52a0fc748ae4a25cf0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:31:03 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:34:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:34:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:34:33 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:34:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322c98bdb14c28d0b5869f41698820d62eabf2e257800da6fa66ff4f17606f23`  
		Last Modified: Thu, 14 Jan 2021 00:59:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e48c6d94fb782acb7b4dc1290faf8c878269b15b9e16293486a5638263c2d8`  
		Last Modified: Thu, 14 Jan 2021 00:59:47 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b0783fa10e8c1d7e4f627b97660f72c5c4f9949ebecfd58af8b34176f79009`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7a8d9c6e1146c13c0f64c47a9fdbd92c2802d228f842c64ff95e7ee67c0a8`  
		Last Modified: Thu, 14 Jan 2021 01:04:16 GMT  
		Size: 234.8 MB (234836390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1863d635dc8311d270ec8a6e3b7ece81eb4357cedbc7160fe58826002f181872`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118baad55a6f99b1acf8a65f36f502a179af8657666d6fd3a782db7266cb561`  
		Last Modified: Thu, 14 Jan 2021 00:59:46 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1f370df1c211a9cadb44a5fd531f53bf58e480df62d0f7acd7c348b578963`  
		Last Modified: Thu, 14 Jan 2021 00:59:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:1b9e1c2cc2e5cca86c706bd706f20568943ad81f6cc427636fcbcf5a8cf7ee9e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6029479083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1969addeb88f3b28d316a642745777fb088614191093025a93670be55d11b1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:34:45 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:38:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:38:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:38:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:39:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268fad4c2c60d1a5eee3ffa02942be8417db10862183c4a8de139ce38d76b42f`  
		Last Modified: Thu, 14 Jan 2021 01:04:47 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574240b920d1e70836565b0cb8167d0025f514dd9068a69974d5d2b258de4d`  
		Last Modified: Thu, 14 Jan 2021 01:04:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704f5df313ebfbb316d9e294be996801c1e4c2ae4da0446e1c3160134bf5cc50`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10bff8dc22cd39d534926404ce75b9a04689d9c9bdfafb6861111cc0972fea8`  
		Last Modified: Thu, 14 Jan 2021 01:08:55 GMT  
		Size: 235.6 MB (235577098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d49ac5bfb0015308d470e3638d64230ec947466b7d2e9e2ca0b5ce64c371b6`  
		Last Modified: Thu, 14 Jan 2021 01:04:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd6e1ff01caf85c900bcf6f7c979b463586791d084c6cb67773ffed35135357`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b66fee24b0f0b4659dc51e91583c75c7e80f7ffa051e2ec710808d07f844d`  
		Last Modified: Thu, 14 Jan 2021 01:04:42 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0fbf918baaba9f3cec5268c6d37531bdf32471c9a58cbdfb61527fe8fbbaa07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:3d52f3757af0a7f9da0ead5abafb6b36d2f42c5ebe0a744c9f59fc9687103295
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2670616546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e6d7d88184b5b2147925eea1a075221df38e6aeb4c6ba52a0fc748ae4a25cf0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:31:03 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:31:04 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:34:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:34:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:34:33 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:34:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322c98bdb14c28d0b5869f41698820d62eabf2e257800da6fa66ff4f17606f23`  
		Last Modified: Thu, 14 Jan 2021 00:59:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e48c6d94fb782acb7b4dc1290faf8c878269b15b9e16293486a5638263c2d8`  
		Last Modified: Thu, 14 Jan 2021 00:59:47 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b0783fa10e8c1d7e4f627b97660f72c5c4f9949ebecfd58af8b34176f79009`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7a8d9c6e1146c13c0f64c47a9fdbd92c2802d228f842c64ff95e7ee67c0a8`  
		Last Modified: Thu, 14 Jan 2021 01:04:16 GMT  
		Size: 234.8 MB (234836390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1863d635dc8311d270ec8a6e3b7ece81eb4357cedbc7160fe58826002f181872`  
		Last Modified: Thu, 14 Jan 2021 00:59:44 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118baad55a6f99b1acf8a65f36f502a179af8657666d6fd3a782db7266cb561`  
		Last Modified: Thu, 14 Jan 2021 00:59:46 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1f370df1c211a9cadb44a5fd531f53bf58e480df62d0f7acd7c348b578963`  
		Last Modified: Thu, 14 Jan 2021 00:59:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:4631ed2bd0f02e99bf90bc7434db1699f5717c319e384a3c5f964026c2416768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:1b9e1c2cc2e5cca86c706bd706f20568943ad81f6cc427636fcbcf5a8cf7ee9e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6029479083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d1969addeb88f3b28d316a642745777fb088614191093025a93670be55d11b1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:34:45 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Thu, 14 Jan 2021 00:34:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Thu, 14 Jan 2021 00:38:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:38:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:38:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:39:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268fad4c2c60d1a5eee3ffa02942be8417db10862183c4a8de139ce38d76b42f`  
		Last Modified: Thu, 14 Jan 2021 01:04:47 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574240b920d1e70836565b0cb8167d0025f514dd9068a69974d5d2b258de4d`  
		Last Modified: Thu, 14 Jan 2021 01:04:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704f5df313ebfbb316d9e294be996801c1e4c2ae4da0446e1c3160134bf5cc50`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10bff8dc22cd39d534926404ce75b9a04689d9c9bdfafb6861111cc0972fea8`  
		Last Modified: Thu, 14 Jan 2021 01:08:55 GMT  
		Size: 235.6 MB (235577098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d49ac5bfb0015308d470e3638d64230ec947466b7d2e9e2ca0b5ce64c371b6`  
		Last Modified: Thu, 14 Jan 2021 01:04:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd6e1ff01caf85c900bcf6f7c979b463586791d084c6cb67773ffed35135357`  
		Last Modified: Thu, 14 Jan 2021 01:04:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b66fee24b0f0b4659dc51e91583c75c7e80f7ffa051e2ec710808d07f844d`  
		Last Modified: Thu, 14 Jan 2021 01:04:42 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:1ea6e4fb08cc9f00b89d3db37a64256266018d252fdbe2b319587cfa18d6ccfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:d6b5eecd9cc3058e4fb96231d67fb6bebd1cf3ac6f1fb8d0a60b1428872a57b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156112747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5323653a57085662bb404d44b61b663c3ad7485b4b04cfcdf8142215d14df946`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:21:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:21:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:21:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:21:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:21:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 21 Jan 2021 10:22:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:22:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:22:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:01 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:01 GMT
ENV MONGO_MAJOR=4.0
# Thu, 21 Jan 2021 10:22:02 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 21 Jan 2021 10:22:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:22:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:22:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:22:21 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:22:21 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:22:22 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:22:22 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27db06de4cbd883f7f8a71875553c592acab09881993b9bfcea34c13fc3324`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbecf0ce3761b56377a68abeb11e96c614b1e5258a335f7cb391884cd66f8cb1`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 2.9 MB (2920165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce97543d924d1319df58ac30e0739ca83f56c801effbb8a432fa8922772f4618`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 1.3 MB (1305584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7299669aa5f56bd19167ebdd0ed0cff061f4f9d9e12f1e6c15ce1ebb8d6a0986`  
		Last Modified: Thu, 21 Jan 2021 10:24:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4269ba38e222385bbc1282954ab869eb75e0e5bb3c1a29b8ad099c1d9ff1b39c`  
		Last Modified: Thu, 21 Jan 2021 10:24:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09264a562b57502b707476cea86b9deda6c6317b2e6cb33ccfedf68c801dc973`  
		Last Modified: Thu, 21 Jan 2021 10:24:58 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6bda190fde0bcecd34358c67051c874ffcd7a879b0b1ca9f10c4d1ef7590d`  
		Last Modified: Thu, 21 Jan 2021 10:25:19 GMT  
		Size: 105.9 MB (105914783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feafd2669d078147527d8449eb8c5e67d0440d398880bb621b5984d107d70967`  
		Last Modified: Thu, 21 Jan 2021 10:24:56 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b490a7d89210b3938d48f47fc8e24c055521a3698fbd88d96902b7e100a709`  
		Last Modified: Thu, 21 Jan 2021 10:24:56 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:89ca5fc8233cacf64b807339363dae970e66431153d33c5aed085dd517d71780
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144864314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0877e91206551ce59ec4e3a7223fc27e5fbb751d438d6f681b10a467083e945b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:50:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:51:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:51:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:51:10 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:51:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:51:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:52:45 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 21 Jan 2021 05:52:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:52:47 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:52:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:52:49 GMT
ENV MONGO_MAJOR=4.0
# Thu, 21 Jan 2021 05:52:50 GMT
ENV MONGO_VERSION=4.0.22
# Thu, 21 Jan 2021 05:52:51 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:53:23 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:53:26 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:53:26 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:53:27 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:53:28 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:53:29 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b26ef0aeab8022d5431105a8f1035fe0257b2ffcdb47d8001991d16f78c23`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c5cced802180d13930db9529191cf993e09f92c58d488c439d2f857665b2fb`  
		Last Modified: Thu, 21 Jan 2021 05:56:36 GMT  
		Size: 2.4 MB (2447664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191641f00320db17c756575cca7186902b376a68bd5bd8d594b72aa43b6b323`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 1.2 MB (1232282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7967e13dbce2f43520898cff9c51418dc809c0f94a546ddaa71d4950813764e4`  
		Last Modified: Thu, 21 Jan 2021 05:56:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b0c8486feab611ac6970c3c8b66319e41a420989534cef3ee891dc82d0c66d`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208ae58d870775a30f78775d29b6eca77bd4596309b196231d41d0f6d00a1df`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cd462b9c75d9dc145a81e4fed8cbf5cd29c1a12c720b4ea213b4612f934b7`  
		Last Modified: Thu, 21 Jan 2021 05:57:30 GMT  
		Size: 100.3 MB (100289261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4cc58789aa6a6c634b35d002d0fe11838513f31b45fa3bb1ce3cdd2e846a0a`  
		Last Modified: Thu, 21 Jan 2021 05:57:09 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed5f0a81ca68f0368b7f76dfae5c8fc7b58d7dc990c704226fc3aa27d7129d8`  
		Last Modified: Thu, 21 Jan 2021 05:57:08 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:3ac00a92dd5771a216076da32000c6f65d7173d55f799d3a7aae12dd75a2f751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:1764d35927b4a0bb2b9ec176a9a09c1bd91402723e2d556f960037f6b0935d7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165064238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91262bc8eca49dfa55ca8e711dcb848c7da7f729dc0cc6ad236841be0f2d3234`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:22:54 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 21 Jan 2021 10:22:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:22:55 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:22:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:56 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:56 GMT
ENV MONGO_MAJOR=4.2
# Thu, 21 Jan 2021 10:22:56 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 21 Jan 2021 10:22:57 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:15 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:16 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:17 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:17 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:17 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:17 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f530ac8a5c0aa2e4935a19e2cad815557e0e6694d74704eebed1f7d36560381`  
		Last Modified: Thu, 21 Jan 2021 10:25:29 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b9a2e794c4f61048c658fb4c257da20c12f1435f70ccd9eca786fc0535a771`  
		Last Modified: Thu, 21 Jan 2021 10:25:29 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6c8ba34dc4a288b9acebe47e7c2727b15034cdddb51a9badebd762d9a9012`  
		Last Modified: Thu, 21 Jan 2021 10:25:49 GMT  
		Size: 129.5 MB (129527627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4a2a00a92c22b32206466ec5ce3b2aec0bfbbe96a4b8618a55afd6d599df1`  
		Last Modified: Thu, 21 Jan 2021 10:25:29 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef25165262d25c3dfb7226269d83c4b44c4b1a9e0ce11e150b95fd7ef6dcf8b5`  
		Last Modified: Thu, 21 Jan 2021 10:25:30 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:acbd4e9ac5e59de7c542f61314c927313c95c57733c2ee0022a1f9c4a442b673
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155071391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026e405dd540f30cbe24b075410eef3474fa57d2b898d6b527b6de4afa917960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 21 Jan 2021 05:54:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:54:30 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:54:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:54:31 GMT
ENV MONGO_MAJOR=4.2
# Mon, 25 Jan 2021 20:46:49 GMT
ENV MONGO_VERSION=4.2.12
# Mon, 25 Jan 2021 20:46:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 25 Jan 2021 20:47:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 25 Jan 2021 20:47:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 25 Jan 2021 20:47:22 GMT
VOLUME [/data/db /data/configdb]
# Mon, 25 Jan 2021 20:47:23 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Mon, 25 Jan 2021 20:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:47:24 GMT
EXPOSE 27017
# Mon, 25 Jan 2021 20:47:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b872df90fccfca7b5f784c6857d733b3beb83d74e19f533b7a6503b4402d15`  
		Last Modified: Thu, 21 Jan 2021 05:57:42 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f061b167f19efaff7cb68ddd4db98e8852e23a12b33a918f77ed08dee6f085`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e6bb6c82966d4ff7d2b4f315dc78e7d312e1ed1e0f577c995e20278b61195`  
		Last Modified: Mon, 25 Jan 2021 20:48:51 GMT  
		Size: 123.3 MB (123300686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43035b7594c0a22f9220901747e769efdd20f4d179aa4ac5688b4c50a7a2d82`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc0c5535500559fb0694cdc1a59d33e2cd82705945fa4af2074146f0343e1e4`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:10e04ac2077cf7704d360e70c5415d6e367a1230ce624aea236ff7bec27cda82
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2725925528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c31ce926497c787585e9ecebda83e2cad04a25eae404971432eeffa6a63de3c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:39:12 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 14 Jan 2021 00:39:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Thu, 14 Jan 2021 00:39:14 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Thu, 14 Jan 2021 00:43:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:43:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:43:16 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:43:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea12fdda5d64e79cc584dacdc982ad4e645211622237179e34e657432ee2c8b1`  
		Last Modified: Thu, 14 Jan 2021 01:09:14 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42746d32a851b64c9d0362b9e6c6576f2ccb3e5e55556f7e84f28fbee049e85c`  
		Last Modified: Thu, 14 Jan 2021 01:09:14 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d440410878c390f4208def19a5aab2128d47fbbc6b9a19cf11a80734e4ae36`  
		Last Modified: Thu, 14 Jan 2021 01:09:10 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f207294d0bc6db890ddc1c5f3d43fc2ebc9de7ae4d53d80aa6493ebfa29ca99`  
		Last Modified: Thu, 14 Jan 2021 01:10:10 GMT  
		Size: 290.1 MB (290145428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de39960d13fa93c872ece88be13f62141bf0654381a31b737e10be20c2fca30`  
		Last Modified: Thu, 14 Jan 2021 01:09:11 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfd85f050512c560ab167eff165f2139dc616c708a5c1c8141fbe617536f80d`  
		Last Modified: Thu, 14 Jan 2021 01:09:12 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d5b482bb999584adb09a66194a5ba22497e817b8e59b8e87100163a1d120e9`  
		Last Modified: Thu, 14 Jan 2021 01:09:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:33b8853f67c2614275a7c4de4068c3c37ddd2ead022433d6625161f16c4c82d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6084786310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:882944b0f72cc0e638ad79d7931f6eece075d0da94f8ced2e1b39e45541d4d73`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:43:24 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 14 Jan 2021 00:43:25 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Thu, 14 Jan 2021 00:43:25 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Thu, 14 Jan 2021 00:48:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:48:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:48:17 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:48:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c39875212e32a18b9baf465517a5439d9526b37d9fa92a57a3ef1f5f20369f`  
		Last Modified: Thu, 14 Jan 2021 01:10:35 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d988f0e467639b637e222e1102fef5291988b09c2bcfd37bb31cd50eff3c4a`  
		Last Modified: Thu, 14 Jan 2021 01:10:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb8a98a7d542dca44865e57608698f8e2749e78cbbae0fe29bade4a9c2cb01a`  
		Last Modified: Thu, 14 Jan 2021 01:10:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf10c8dadc42191322523ab8a90ce5a70e2644ee57c142486d2478fc2fdc8da`  
		Last Modified: Thu, 14 Jan 2021 01:11:28 GMT  
		Size: 290.9 MB (290884288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9f7671a8ad072f3ef6c2736e18ffd84e1090a25d6b91d9bfa25be72849181`  
		Last Modified: Thu, 14 Jan 2021 01:10:33 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce1342fee92193706d9fa343dafc3e55d7ff5f8f17a96bf5066280c338fdbee`  
		Last Modified: Thu, 14 Jan 2021 01:10:32 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdba5431a35ddab4de7301e9aae85b21e6261291f7f75bbb26334d72a2921094`  
		Last Modified: Thu, 14 Jan 2021 01:10:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.12`

```console
$ docker pull mongo@sha256:4c73389757b3b10f5b061de67f5453cf843c30637e65d06ae0b876e9dc273bc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mongo:4.2.12` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:acbd4e9ac5e59de7c542f61314c927313c95c57733c2ee0022a1f9c4a442b673
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155071391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026e405dd540f30cbe24b075410eef3474fa57d2b898d6b527b6de4afa917960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 21 Jan 2021 05:54:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:54:30 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:54:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:54:31 GMT
ENV MONGO_MAJOR=4.2
# Mon, 25 Jan 2021 20:46:49 GMT
ENV MONGO_VERSION=4.2.12
# Mon, 25 Jan 2021 20:46:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 25 Jan 2021 20:47:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 25 Jan 2021 20:47:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 25 Jan 2021 20:47:22 GMT
VOLUME [/data/db /data/configdb]
# Mon, 25 Jan 2021 20:47:23 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Mon, 25 Jan 2021 20:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:47:24 GMT
EXPOSE 27017
# Mon, 25 Jan 2021 20:47:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b872df90fccfca7b5f784c6857d733b3beb83d74e19f533b7a6503b4402d15`  
		Last Modified: Thu, 21 Jan 2021 05:57:42 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f061b167f19efaff7cb68ddd4db98e8852e23a12b33a918f77ed08dee6f085`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e6bb6c82966d4ff7d2b4f315dc78e7d312e1ed1e0f577c995e20278b61195`  
		Last Modified: Mon, 25 Jan 2021 20:48:51 GMT  
		Size: 123.3 MB (123300686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43035b7594c0a22f9220901747e769efdd20f4d179aa4ac5688b4c50a7a2d82`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc0c5535500559fb0694cdc1a59d33e2cd82705945fa4af2074146f0343e1e4`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.12-bionic`

```console
$ docker pull mongo@sha256:4c73389757b3b10f5b061de67f5453cf843c30637e65d06ae0b876e9dc273bc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mongo:4.2.12-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:acbd4e9ac5e59de7c542f61314c927313c95c57733c2ee0022a1f9c4a442b673
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155071391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026e405dd540f30cbe24b075410eef3474fa57d2b898d6b527b6de4afa917960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 21 Jan 2021 05:54:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:54:30 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:54:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:54:31 GMT
ENV MONGO_MAJOR=4.2
# Mon, 25 Jan 2021 20:46:49 GMT
ENV MONGO_VERSION=4.2.12
# Mon, 25 Jan 2021 20:46:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 25 Jan 2021 20:47:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 25 Jan 2021 20:47:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 25 Jan 2021 20:47:22 GMT
VOLUME [/data/db /data/configdb]
# Mon, 25 Jan 2021 20:47:23 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Mon, 25 Jan 2021 20:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:47:24 GMT
EXPOSE 27017
# Mon, 25 Jan 2021 20:47:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b872df90fccfca7b5f784c6857d733b3beb83d74e19f533b7a6503b4402d15`  
		Last Modified: Thu, 21 Jan 2021 05:57:42 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f061b167f19efaff7cb68ddd4db98e8852e23a12b33a918f77ed08dee6f085`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e6bb6c82966d4ff7d2b4f315dc78e7d312e1ed1e0f577c995e20278b61195`  
		Last Modified: Mon, 25 Jan 2021 20:48:51 GMT  
		Size: 123.3 MB (123300686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43035b7594c0a22f9220901747e769efdd20f4d179aa4ac5688b4c50a7a2d82`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc0c5535500559fb0694cdc1a59d33e2cd82705945fa4af2074146f0343e1e4`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.12-windowsservercore`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2.12-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2.12-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:789a0f6e986fdff7299c2949a090b88b46f078866e8dfb4007bdfa5682b66192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:1764d35927b4a0bb2b9ec176a9a09c1bd91402723e2d556f960037f6b0935d7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165064238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91262bc8eca49dfa55ca8e711dcb848c7da7f729dc0cc6ad236841be0f2d3234`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:22:54 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 21 Jan 2021 10:22:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:22:55 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:22:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:56 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:22:56 GMT
ENV MONGO_MAJOR=4.2
# Thu, 21 Jan 2021 10:22:56 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 21 Jan 2021 10:22:57 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:15 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:16 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:17 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:17 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:17 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:17 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f530ac8a5c0aa2e4935a19e2cad815557e0e6694d74704eebed1f7d36560381`  
		Last Modified: Thu, 21 Jan 2021 10:25:29 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b9a2e794c4f61048c658fb4c257da20c12f1435f70ccd9eca786fc0535a771`  
		Last Modified: Thu, 21 Jan 2021 10:25:29 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6c8ba34dc4a288b9acebe47e7c2727b15034cdddb51a9badebd762d9a9012`  
		Last Modified: Thu, 21 Jan 2021 10:25:49 GMT  
		Size: 129.5 MB (129527627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4a2a00a92c22b32206466ec5ce3b2aec0bfbbe96a4b8618a55afd6d599df1`  
		Last Modified: Thu, 21 Jan 2021 10:25:29 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef25165262d25c3dfb7226269d83c4b44c4b1a9e0ce11e150b95fd7ef6dcf8b5`  
		Last Modified: Thu, 21 Jan 2021 10:25:30 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:acbd4e9ac5e59de7c542f61314c927313c95c57733c2ee0022a1f9c4a442b673
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155071391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026e405dd540f30cbe24b075410eef3474fa57d2b898d6b527b6de4afa917960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:26 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 21 Jan 2021 05:54:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:54:30 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:54:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:54:31 GMT
ENV MONGO_MAJOR=4.2
# Mon, 25 Jan 2021 20:46:49 GMT
ENV MONGO_VERSION=4.2.12
# Mon, 25 Jan 2021 20:46:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 25 Jan 2021 20:47:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 25 Jan 2021 20:47:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 25 Jan 2021 20:47:22 GMT
VOLUME [/data/db /data/configdb]
# Mon, 25 Jan 2021 20:47:23 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Mon, 25 Jan 2021 20:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:47:24 GMT
EXPOSE 27017
# Mon, 25 Jan 2021 20:47:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b872df90fccfca7b5f784c6857d733b3beb83d74e19f533b7a6503b4402d15`  
		Last Modified: Thu, 21 Jan 2021 05:57:42 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f061b167f19efaff7cb68ddd4db98e8852e23a12b33a918f77ed08dee6f085`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e6bb6c82966d4ff7d2b4f315dc78e7d312e1ed1e0f577c995e20278b61195`  
		Last Modified: Mon, 25 Jan 2021 20:48:51 GMT  
		Size: 123.3 MB (123300686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43035b7594c0a22f9220901747e769efdd20f4d179aa4ac5688b4c50a7a2d82`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc0c5535500559fb0694cdc1a59d33e2cd82705945fa4af2074146f0343e1e4`  
		Last Modified: Mon, 25 Jan 2021 20:48:18 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:1a5c4042fdaf28b9ae712c3883c9c0a9207be9929ec3400f3aa7a5e16d9f30a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:10e04ac2077cf7704d360e70c5415d6e367a1230ce624aea236ff7bec27cda82
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2725925528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c31ce926497c787585e9ecebda83e2cad04a25eae404971432eeffa6a63de3c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:39:12 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 14 Jan 2021 00:39:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Thu, 14 Jan 2021 00:39:14 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Thu, 14 Jan 2021 00:43:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:43:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:43:16 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:43:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea12fdda5d64e79cc584dacdc982ad4e645211622237179e34e657432ee2c8b1`  
		Last Modified: Thu, 14 Jan 2021 01:09:14 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42746d32a851b64c9d0362b9e6c6576f2ccb3e5e55556f7e84f28fbee049e85c`  
		Last Modified: Thu, 14 Jan 2021 01:09:14 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d440410878c390f4208def19a5aab2128d47fbbc6b9a19cf11a80734e4ae36`  
		Last Modified: Thu, 14 Jan 2021 01:09:10 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f207294d0bc6db890ddc1c5f3d43fc2ebc9de7ae4d53d80aa6493ebfa29ca99`  
		Last Modified: Thu, 14 Jan 2021 01:10:10 GMT  
		Size: 290.1 MB (290145428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de39960d13fa93c872ece88be13f62141bf0654381a31b737e10be20c2fca30`  
		Last Modified: Thu, 14 Jan 2021 01:09:11 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfd85f050512c560ab167eff165f2139dc616c708a5c1c8141fbe617536f80d`  
		Last Modified: Thu, 14 Jan 2021 01:09:12 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d5b482bb999584adb09a66194a5ba22497e817b8e59b8e87100163a1d120e9`  
		Last Modified: Thu, 14 Jan 2021 01:09:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:33b8853f67c2614275a7c4de4068c3c37ddd2ead022433d6625161f16c4c82d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6084786310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:882944b0f72cc0e638ad79d7931f6eece075d0da94f8ced2e1b39e45541d4d73`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:43:24 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 14 Jan 2021 00:43:25 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Thu, 14 Jan 2021 00:43:25 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Thu, 14 Jan 2021 00:48:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:48:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:48:17 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:48:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c39875212e32a18b9baf465517a5439d9526b37d9fa92a57a3ef1f5f20369f`  
		Last Modified: Thu, 14 Jan 2021 01:10:35 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d988f0e467639b637e222e1102fef5291988b09c2bcfd37bb31cd50eff3c4a`  
		Last Modified: Thu, 14 Jan 2021 01:10:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb8a98a7d542dca44865e57608698f8e2749e78cbbae0fe29bade4a9c2cb01a`  
		Last Modified: Thu, 14 Jan 2021 01:10:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf10c8dadc42191322523ab8a90ce5a70e2644ee57c142486d2478fc2fdc8da`  
		Last Modified: Thu, 14 Jan 2021 01:11:28 GMT  
		Size: 290.9 MB (290884288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9f7671a8ad072f3ef6c2736e18ffd84e1090a25d6b91d9bfa25be72849181`  
		Last Modified: Thu, 14 Jan 2021 01:10:33 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce1342fee92193706d9fa343dafc3e55d7ff5f8f17a96bf5066280c338fdbee`  
		Last Modified: Thu, 14 Jan 2021 01:10:32 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdba5431a35ddab4de7301e9aae85b21e6261291f7f75bbb26334d72a2921094`  
		Last Modified: Thu, 14 Jan 2021 01:10:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:1d21331de1531fd4b4a7311f7cd219e96391fa8d3e17c9908c98e8c3fe7393b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:10e04ac2077cf7704d360e70c5415d6e367a1230ce624aea236ff7bec27cda82
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2725925528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c31ce926497c787585e9ecebda83e2cad04a25eae404971432eeffa6a63de3c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:39:12 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 14 Jan 2021 00:39:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Thu, 14 Jan 2021 00:39:14 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Thu, 14 Jan 2021 00:43:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:43:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:43:16 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:43:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea12fdda5d64e79cc584dacdc982ad4e645211622237179e34e657432ee2c8b1`  
		Last Modified: Thu, 14 Jan 2021 01:09:14 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42746d32a851b64c9d0362b9e6c6576f2ccb3e5e55556f7e84f28fbee049e85c`  
		Last Modified: Thu, 14 Jan 2021 01:09:14 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d440410878c390f4208def19a5aab2128d47fbbc6b9a19cf11a80734e4ae36`  
		Last Modified: Thu, 14 Jan 2021 01:09:10 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f207294d0bc6db890ddc1c5f3d43fc2ebc9de7ae4d53d80aa6493ebfa29ca99`  
		Last Modified: Thu, 14 Jan 2021 01:10:10 GMT  
		Size: 290.1 MB (290145428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de39960d13fa93c872ece88be13f62141bf0654381a31b737e10be20c2fca30`  
		Last Modified: Thu, 14 Jan 2021 01:09:11 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfd85f050512c560ab167eff165f2139dc616c708a5c1c8141fbe617536f80d`  
		Last Modified: Thu, 14 Jan 2021 01:09:12 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d5b482bb999584adb09a66194a5ba22497e817b8e59b8e87100163a1d120e9`  
		Last Modified: Thu, 14 Jan 2021 01:09:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:b2e14958a51587687de85f039216264157c71d8ed4ec4bf91ef1542e7aa123d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:33b8853f67c2614275a7c4de4068c3c37ddd2ead022433d6625161f16c4c82d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6084786310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:882944b0f72cc0e638ad79d7931f6eece075d0da94f8ced2e1b39e45541d4d73`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:43:24 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 14 Jan 2021 00:43:25 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Thu, 14 Jan 2021 00:43:25 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Thu, 14 Jan 2021 00:48:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:48:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:48:17 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:48:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c39875212e32a18b9baf465517a5439d9526b37d9fa92a57a3ef1f5f20369f`  
		Last Modified: Thu, 14 Jan 2021 01:10:35 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d988f0e467639b637e222e1102fef5291988b09c2bcfd37bb31cd50eff3c4a`  
		Last Modified: Thu, 14 Jan 2021 01:10:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb8a98a7d542dca44865e57608698f8e2749e78cbbae0fe29bade4a9c2cb01a`  
		Last Modified: Thu, 14 Jan 2021 01:10:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf10c8dadc42191322523ab8a90ce5a70e2644ee57c142486d2478fc2fdc8da`  
		Last Modified: Thu, 14 Jan 2021 01:11:28 GMT  
		Size: 290.9 MB (290884288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9f7671a8ad072f3ef6c2736e18ffd84e1090a25d6b91d9bfa25be72849181`  
		Last Modified: Thu, 14 Jan 2021 01:10:33 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce1342fee92193706d9fa343dafc3e55d7ff5f8f17a96bf5066280c338fdbee`  
		Last Modified: Thu, 14 Jan 2021 01:10:32 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdba5431a35ddab4de7301e9aae85b21e6261291f7f75bbb26334d72a2921094`  
		Last Modified: Thu, 14 Jan 2021 01:10:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4`

```console
$ docker pull mongo@sha256:88e0308671a06d4ee7da41f87944ba66355b4ee3d57d57caf92f5e1938736abd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.4` - linux; amd64

```console
$ docker pull mongo@sha256:06ba42906e0346c15a795ff6ebcb3ac88be0f85aa899a6225979029188e312c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178222610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8e14b1fda68aedb435fec2a6eaa326cf5633fc57b7e28b5cc37d938ead9edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:23:24 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 10:23:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:26 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 10:23:28 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:52 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:52 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca70046d298d7aac215eecead78d18f8f28e11eaea6db7f35c945e64a43124`  
		Last Modified: Thu, 21 Jan 2021 10:25:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a541da2a89089f196a998312c16f37f8ee11251f88d764ce95274dd29d5a3`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18edd0c32639b9f81da45ecc082e23f67c7eb02bc3a1216622dfe181c852f505`  
		Last Modified: Thu, 21 Jan 2021 10:26:20 GMT  
		Size: 142.7 MB (142686014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86830e28cf719e7b6459badd7a5ade676e32d9b08c004774f65dce25bc639636`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1d772417d960c2608d622279c356232f0b70a0b82c7129bf57df7f4c1aeea`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:35d866a5fd70ff9b9cd520ad48bc4250f1a4e05171b205fcfc68fe9c51efa8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168151561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095aea9826c2c421ae2b1c4299766ba6461174f3a901019cb427b1d1cf54f5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:55:16 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 05:55:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:55:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:55:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:21 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 05:55:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:55:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:55:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:55:55 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:55:56 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:57 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:55:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f46ba3c06d737a4d0e64c1f3db503400ee0eb1b4b4bb586b0bd7f9ded60c3a`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144bd8644f0fbdd12fa8e9850c9036f763fb7720a1a580a0ad88bd9c35fc4684`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250692aff7a7255ff3544fd94c39f0a2896636ced434869481c1029047068c4`  
		Last Modified: Thu, 21 Jan 2021 05:58:51 GMT  
		Size: 136.4 MB (136380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f467e359b3608c8a4425b25553555612e50e64f8e954c382195fcf3cd28401d0`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a524c0aa3acb289bb84a7514ddf6c6ac6cb5feb52a04d253aedc50de4a73488e`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; s390x

```console
$ docker pull mongo@sha256:9c0b379fa79bc55520a9badaf4ac04a213d55e2e76c1f453261e7010e62c1b82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173132528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc71b87dda565765e825ef3f366cd24b6512c3c1495ee26e640d82412d9ed5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 04:00:45 GMT
ADD file:d443bbf06b974365e3cb2d99eea08d454059cf95b82a6023e4260fba5ead568e in / 
# Thu, 21 Jan 2021 04:00:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:00:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:00:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:00:56 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 04:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:39:49 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 04:39:50 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 04:40:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 04:40:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 04:40:15 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 04:40:17 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 04:40:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 04:41:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 04:41:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 04:41:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 04:41:25 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 04:41:27 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 04:41:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1a4e1c3f599543fe1043f321c3c5e14f5ca6073cba211f2144b569c5d0cff014`  
		Last Modified: Thu, 21 Jan 2021 04:03:17 GMT  
		Size: 25.4 MB (25381801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1202f2791a7390dbd7197d4cfde724e184be1b2f9d4791890fb64341336f889e`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c44bad24828f92a8ff703d4d356f2969f0c1de9f6d852d3cec338a3aff6265`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad237e33328657490128a3945e880b746ebd50c75cc14cb7e6cb1e2c60e8a1b`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2023f0f19357e97e77398f90b92a5736e2f71e3413a2fdc91330fc05461250`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 2.7 MB (2721180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb06349457fa157b55404be7a301c14dce1915009bad7fa29e12925d5821993`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 5.7 MB (5746846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33428088ab5395067d4b3d3b8dee47ab7f7237cdd0a4df0e3f6b8521c3fb839b`  
		Last Modified: Thu, 21 Jan 2021 04:42:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3464b0455ffb640246507864b1476076c6d50b7235fbc64c3bfd8e5660f4537`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684dd6070aa89f7d64e27f891d77a5fea632b893241ff66da06f16e54b3c96a6`  
		Last Modified: Thu, 21 Jan 2021 04:42:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c67edb3d568d86357a630edc1923d8fa70e3eea8bc5920edcf29dab66f11d4`  
		Last Modified: Thu, 21 Jan 2021 04:42:22 GMT  
		Size: 139.3 MB (139273378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e1ffd4eb011cb4d1416bf7f49751b13a4dfb5b0c37238e672290617b87dcf4`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efad1d47d721328a8ba57a39bc62b6560d33378f004345c4e3b5c39baf6fd48`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3`

```console
$ docker pull mongo@sha256:88e0308671a06d4ee7da41f87944ba66355b4ee3d57d57caf92f5e1938736abd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.4.3` - linux; amd64

```console
$ docker pull mongo@sha256:06ba42906e0346c15a795ff6ebcb3ac88be0f85aa899a6225979029188e312c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178222610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8e14b1fda68aedb435fec2a6eaa326cf5633fc57b7e28b5cc37d938ead9edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:23:24 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 10:23:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:26 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 10:23:28 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:52 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:52 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca70046d298d7aac215eecead78d18f8f28e11eaea6db7f35c945e64a43124`  
		Last Modified: Thu, 21 Jan 2021 10:25:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a541da2a89089f196a998312c16f37f8ee11251f88d764ce95274dd29d5a3`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18edd0c32639b9f81da45ecc082e23f67c7eb02bc3a1216622dfe181c852f505`  
		Last Modified: Thu, 21 Jan 2021 10:26:20 GMT  
		Size: 142.7 MB (142686014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86830e28cf719e7b6459badd7a5ade676e32d9b08c004774f65dce25bc639636`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1d772417d960c2608d622279c356232f0b70a0b82c7129bf57df7f4c1aeea`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:35d866a5fd70ff9b9cd520ad48bc4250f1a4e05171b205fcfc68fe9c51efa8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168151561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095aea9826c2c421ae2b1c4299766ba6461174f3a901019cb427b1d1cf54f5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:55:16 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 05:55:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:55:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:55:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:21 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 05:55:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:55:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:55:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:55:55 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:55:56 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:57 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:55:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f46ba3c06d737a4d0e64c1f3db503400ee0eb1b4b4bb586b0bd7f9ded60c3a`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144bd8644f0fbdd12fa8e9850c9036f763fb7720a1a580a0ad88bd9c35fc4684`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250692aff7a7255ff3544fd94c39f0a2896636ced434869481c1029047068c4`  
		Last Modified: Thu, 21 Jan 2021 05:58:51 GMT  
		Size: 136.4 MB (136380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f467e359b3608c8a4425b25553555612e50e64f8e954c382195fcf3cd28401d0`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a524c0aa3acb289bb84a7514ddf6c6ac6cb5feb52a04d253aedc50de4a73488e`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3` - linux; s390x

```console
$ docker pull mongo@sha256:9c0b379fa79bc55520a9badaf4ac04a213d55e2e76c1f453261e7010e62c1b82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173132528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc71b87dda565765e825ef3f366cd24b6512c3c1495ee26e640d82412d9ed5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 04:00:45 GMT
ADD file:d443bbf06b974365e3cb2d99eea08d454059cf95b82a6023e4260fba5ead568e in / 
# Thu, 21 Jan 2021 04:00:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:00:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:00:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:00:56 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 04:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:39:49 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 04:39:50 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 04:40:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 04:40:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 04:40:15 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 04:40:17 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 04:40:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 04:41:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 04:41:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 04:41:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 04:41:25 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 04:41:27 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 04:41:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1a4e1c3f599543fe1043f321c3c5e14f5ca6073cba211f2144b569c5d0cff014`  
		Last Modified: Thu, 21 Jan 2021 04:03:17 GMT  
		Size: 25.4 MB (25381801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1202f2791a7390dbd7197d4cfde724e184be1b2f9d4791890fb64341336f889e`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c44bad24828f92a8ff703d4d356f2969f0c1de9f6d852d3cec338a3aff6265`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad237e33328657490128a3945e880b746ebd50c75cc14cb7e6cb1e2c60e8a1b`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2023f0f19357e97e77398f90b92a5736e2f71e3413a2fdc91330fc05461250`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 2.7 MB (2721180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb06349457fa157b55404be7a301c14dce1915009bad7fa29e12925d5821993`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 5.7 MB (5746846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33428088ab5395067d4b3d3b8dee47ab7f7237cdd0a4df0e3f6b8521c3fb839b`  
		Last Modified: Thu, 21 Jan 2021 04:42:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3464b0455ffb640246507864b1476076c6d50b7235fbc64c3bfd8e5660f4537`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684dd6070aa89f7d64e27f891d77a5fea632b893241ff66da06f16e54b3c96a6`  
		Last Modified: Thu, 21 Jan 2021 04:42:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c67edb3d568d86357a630edc1923d8fa70e3eea8bc5920edcf29dab66f11d4`  
		Last Modified: Thu, 21 Jan 2021 04:42:22 GMT  
		Size: 139.3 MB (139273378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e1ffd4eb011cb4d1416bf7f49751b13a4dfb5b0c37238e672290617b87dcf4`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efad1d47d721328a8ba57a39bc62b6560d33378f004345c4e3b5c39baf6fd48`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3-bionic`

```console
$ docker pull mongo@sha256:0290400e988ee9856ad321f81781827e0124d13f68cc72d6cad4807f3174946c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.3-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:06ba42906e0346c15a795ff6ebcb3ac88be0f85aa899a6225979029188e312c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178222610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8e14b1fda68aedb435fec2a6eaa326cf5633fc57b7e28b5cc37d938ead9edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:23:24 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 10:23:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:26 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 10:23:28 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:52 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:52 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca70046d298d7aac215eecead78d18f8f28e11eaea6db7f35c945e64a43124`  
		Last Modified: Thu, 21 Jan 2021 10:25:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a541da2a89089f196a998312c16f37f8ee11251f88d764ce95274dd29d5a3`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18edd0c32639b9f81da45ecc082e23f67c7eb02bc3a1216622dfe181c852f505`  
		Last Modified: Thu, 21 Jan 2021 10:26:20 GMT  
		Size: 142.7 MB (142686014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86830e28cf719e7b6459badd7a5ade676e32d9b08c004774f65dce25bc639636`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1d772417d960c2608d622279c356232f0b70a0b82c7129bf57df7f4c1aeea`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:35d866a5fd70ff9b9cd520ad48bc4250f1a4e05171b205fcfc68fe9c51efa8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168151561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095aea9826c2c421ae2b1c4299766ba6461174f3a901019cb427b1d1cf54f5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:55:16 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 05:55:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:55:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:55:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:21 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 05:55:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:55:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:55:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:55:55 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:55:56 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:57 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:55:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f46ba3c06d737a4d0e64c1f3db503400ee0eb1b4b4bb586b0bd7f9ded60c3a`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144bd8644f0fbdd12fa8e9850c9036f763fb7720a1a580a0ad88bd9c35fc4684`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250692aff7a7255ff3544fd94c39f0a2896636ced434869481c1029047068c4`  
		Last Modified: Thu, 21 Jan 2021 05:58:51 GMT  
		Size: 136.4 MB (136380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f467e359b3608c8a4425b25553555612e50e64f8e954c382195fcf3cd28401d0`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a524c0aa3acb289bb84a7514ddf6c6ac6cb5feb52a04d253aedc50de4a73488e`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:9c0b379fa79bc55520a9badaf4ac04a213d55e2e76c1f453261e7010e62c1b82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173132528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc71b87dda565765e825ef3f366cd24b6512c3c1495ee26e640d82412d9ed5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 04:00:45 GMT
ADD file:d443bbf06b974365e3cb2d99eea08d454059cf95b82a6023e4260fba5ead568e in / 
# Thu, 21 Jan 2021 04:00:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:00:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:00:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:00:56 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 04:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:39:49 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 04:39:50 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 04:40:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 04:40:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 04:40:15 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 04:40:17 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 04:40:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 04:41:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 04:41:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 04:41:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 04:41:25 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 04:41:27 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 04:41:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1a4e1c3f599543fe1043f321c3c5e14f5ca6073cba211f2144b569c5d0cff014`  
		Last Modified: Thu, 21 Jan 2021 04:03:17 GMT  
		Size: 25.4 MB (25381801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1202f2791a7390dbd7197d4cfde724e184be1b2f9d4791890fb64341336f889e`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c44bad24828f92a8ff703d4d356f2969f0c1de9f6d852d3cec338a3aff6265`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad237e33328657490128a3945e880b746ebd50c75cc14cb7e6cb1e2c60e8a1b`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2023f0f19357e97e77398f90b92a5736e2f71e3413a2fdc91330fc05461250`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 2.7 MB (2721180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb06349457fa157b55404be7a301c14dce1915009bad7fa29e12925d5821993`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 5.7 MB (5746846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33428088ab5395067d4b3d3b8dee47ab7f7237cdd0a4df0e3f6b8521c3fb839b`  
		Last Modified: Thu, 21 Jan 2021 04:42:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3464b0455ffb640246507864b1476076c6d50b7235fbc64c3bfd8e5660f4537`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684dd6070aa89f7d64e27f891d77a5fea632b893241ff66da06f16e54b3c96a6`  
		Last Modified: Thu, 21 Jan 2021 04:42:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c67edb3d568d86357a630edc1923d8fa70e3eea8bc5920edcf29dab66f11d4`  
		Last Modified: Thu, 21 Jan 2021 04:42:22 GMT  
		Size: 139.3 MB (139273378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e1ffd4eb011cb4d1416bf7f49751b13a4dfb5b0c37238e672290617b87dcf4`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efad1d47d721328a8ba57a39bc62b6560d33378f004345c4e3b5c39baf6fd48`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3-windowsservercore`

```console
$ docker pull mongo@sha256:c411bd2e1a16b2ed7137b3f4dde84bf8f4c920369bf4498fe3d0841e70388434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.4.3-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a218b70c050ffcd70e88e2969459b0b990e9e0f4e32973a5e090ab7785ab7bcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:4.4.3-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:84704a0ba708c7ebe301eefad6f553d9eae46c1640dc29371dc211f22589cc99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.4.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-bionic`

```console
$ docker pull mongo@sha256:0290400e988ee9856ad321f81781827e0124d13f68cc72d6cad4807f3174946c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:06ba42906e0346c15a795ff6ebcb3ac88be0f85aa899a6225979029188e312c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178222610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8e14b1fda68aedb435fec2a6eaa326cf5633fc57b7e28b5cc37d938ead9edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:23:24 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 10:23:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:26 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 10:23:28 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:52 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:52 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca70046d298d7aac215eecead78d18f8f28e11eaea6db7f35c945e64a43124`  
		Last Modified: Thu, 21 Jan 2021 10:25:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a541da2a89089f196a998312c16f37f8ee11251f88d764ce95274dd29d5a3`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18edd0c32639b9f81da45ecc082e23f67c7eb02bc3a1216622dfe181c852f505`  
		Last Modified: Thu, 21 Jan 2021 10:26:20 GMT  
		Size: 142.7 MB (142686014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86830e28cf719e7b6459badd7a5ade676e32d9b08c004774f65dce25bc639636`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1d772417d960c2608d622279c356232f0b70a0b82c7129bf57df7f4c1aeea`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:35d866a5fd70ff9b9cd520ad48bc4250f1a4e05171b205fcfc68fe9c51efa8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168151561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095aea9826c2c421ae2b1c4299766ba6461174f3a901019cb427b1d1cf54f5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:55:16 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 05:55:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:55:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:55:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:21 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 05:55:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:55:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:55:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:55:55 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:55:56 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:57 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:55:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f46ba3c06d737a4d0e64c1f3db503400ee0eb1b4b4bb586b0bd7f9ded60c3a`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144bd8644f0fbdd12fa8e9850c9036f763fb7720a1a580a0ad88bd9c35fc4684`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250692aff7a7255ff3544fd94c39f0a2896636ced434869481c1029047068c4`  
		Last Modified: Thu, 21 Jan 2021 05:58:51 GMT  
		Size: 136.4 MB (136380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f467e359b3608c8a4425b25553555612e50e64f8e954c382195fcf3cd28401d0`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a524c0aa3acb289bb84a7514ddf6c6ac6cb5feb52a04d253aedc50de4a73488e`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:9c0b379fa79bc55520a9badaf4ac04a213d55e2e76c1f453261e7010e62c1b82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173132528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc71b87dda565765e825ef3f366cd24b6512c3c1495ee26e640d82412d9ed5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 04:00:45 GMT
ADD file:d443bbf06b974365e3cb2d99eea08d454059cf95b82a6023e4260fba5ead568e in / 
# Thu, 21 Jan 2021 04:00:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:00:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:00:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:00:56 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 04:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:39:49 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 04:39:50 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 04:40:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 04:40:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 04:40:15 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 04:40:17 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 04:40:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 04:41:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 04:41:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 04:41:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 04:41:25 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 04:41:27 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 04:41:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1a4e1c3f599543fe1043f321c3c5e14f5ca6073cba211f2144b569c5d0cff014`  
		Last Modified: Thu, 21 Jan 2021 04:03:17 GMT  
		Size: 25.4 MB (25381801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1202f2791a7390dbd7197d4cfde724e184be1b2f9d4791890fb64341336f889e`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c44bad24828f92a8ff703d4d356f2969f0c1de9f6d852d3cec338a3aff6265`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad237e33328657490128a3945e880b746ebd50c75cc14cb7e6cb1e2c60e8a1b`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2023f0f19357e97e77398f90b92a5736e2f71e3413a2fdc91330fc05461250`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 2.7 MB (2721180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb06349457fa157b55404be7a301c14dce1915009bad7fa29e12925d5821993`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 5.7 MB (5746846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33428088ab5395067d4b3d3b8dee47ab7f7237cdd0a4df0e3f6b8521c3fb839b`  
		Last Modified: Thu, 21 Jan 2021 04:42:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3464b0455ffb640246507864b1476076c6d50b7235fbc64c3bfd8e5660f4537`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684dd6070aa89f7d64e27f891d77a5fea632b893241ff66da06f16e54b3c96a6`  
		Last Modified: Thu, 21 Jan 2021 04:42:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c67edb3d568d86357a630edc1923d8fa70e3eea8bc5920edcf29dab66f11d4`  
		Last Modified: Thu, 21 Jan 2021 04:42:22 GMT  
		Size: 139.3 MB (139273378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e1ffd4eb011cb4d1416bf7f49751b13a4dfb5b0c37238e672290617b87dcf4`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efad1d47d721328a8ba57a39bc62b6560d33378f004345c4e3b5c39baf6fd48`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore`

```console
$ docker pull mongo@sha256:c411bd2e1a16b2ed7137b3f4dde84bf8f4c920369bf4498fe3d0841e70388434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.4-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a218b70c050ffcd70e88e2969459b0b990e9e0f4e32973a5e090ab7785ab7bcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:4.4-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:84704a0ba708c7ebe301eefad6f553d9eae46c1640dc29371dc211f22589cc99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:0290400e988ee9856ad321f81781827e0124d13f68cc72d6cad4807f3174946c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:06ba42906e0346c15a795ff6ebcb3ac88be0f85aa899a6225979029188e312c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178222610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8e14b1fda68aedb435fec2a6eaa326cf5633fc57b7e28b5cc37d938ead9edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:23:24 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 10:23:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:26 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 10:23:28 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:52 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:52 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca70046d298d7aac215eecead78d18f8f28e11eaea6db7f35c945e64a43124`  
		Last Modified: Thu, 21 Jan 2021 10:25:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a541da2a89089f196a998312c16f37f8ee11251f88d764ce95274dd29d5a3`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18edd0c32639b9f81da45ecc082e23f67c7eb02bc3a1216622dfe181c852f505`  
		Last Modified: Thu, 21 Jan 2021 10:26:20 GMT  
		Size: 142.7 MB (142686014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86830e28cf719e7b6459badd7a5ade676e32d9b08c004774f65dce25bc639636`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1d772417d960c2608d622279c356232f0b70a0b82c7129bf57df7f4c1aeea`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:35d866a5fd70ff9b9cd520ad48bc4250f1a4e05171b205fcfc68fe9c51efa8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168151561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095aea9826c2c421ae2b1c4299766ba6461174f3a901019cb427b1d1cf54f5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:55:16 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 05:55:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:55:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:55:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:21 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 05:55:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:55:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:55:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:55:55 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:55:56 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:57 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:55:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f46ba3c06d737a4d0e64c1f3db503400ee0eb1b4b4bb586b0bd7f9ded60c3a`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144bd8644f0fbdd12fa8e9850c9036f763fb7720a1a580a0ad88bd9c35fc4684`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250692aff7a7255ff3544fd94c39f0a2896636ced434869481c1029047068c4`  
		Last Modified: Thu, 21 Jan 2021 05:58:51 GMT  
		Size: 136.4 MB (136380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f467e359b3608c8a4425b25553555612e50e64f8e954c382195fcf3cd28401d0`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a524c0aa3acb289bb84a7514ddf6c6ac6cb5feb52a04d253aedc50de4a73488e`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:9c0b379fa79bc55520a9badaf4ac04a213d55e2e76c1f453261e7010e62c1b82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173132528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc71b87dda565765e825ef3f366cd24b6512c3c1495ee26e640d82412d9ed5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 04:00:45 GMT
ADD file:d443bbf06b974365e3cb2d99eea08d454059cf95b82a6023e4260fba5ead568e in / 
# Thu, 21 Jan 2021 04:00:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:00:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:00:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:00:56 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 04:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:39:49 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 04:39:50 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 04:40:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 04:40:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 04:40:15 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 04:40:17 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 04:40:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 04:41:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 04:41:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 04:41:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 04:41:25 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 04:41:27 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 04:41:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1a4e1c3f599543fe1043f321c3c5e14f5ca6073cba211f2144b569c5d0cff014`  
		Last Modified: Thu, 21 Jan 2021 04:03:17 GMT  
		Size: 25.4 MB (25381801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1202f2791a7390dbd7197d4cfde724e184be1b2f9d4791890fb64341336f889e`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c44bad24828f92a8ff703d4d356f2969f0c1de9f6d852d3cec338a3aff6265`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad237e33328657490128a3945e880b746ebd50c75cc14cb7e6cb1e2c60e8a1b`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2023f0f19357e97e77398f90b92a5736e2f71e3413a2fdc91330fc05461250`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 2.7 MB (2721180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb06349457fa157b55404be7a301c14dce1915009bad7fa29e12925d5821993`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 5.7 MB (5746846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33428088ab5395067d4b3d3b8dee47ab7f7237cdd0a4df0e3f6b8521c3fb839b`  
		Last Modified: Thu, 21 Jan 2021 04:42:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3464b0455ffb640246507864b1476076c6d50b7235fbc64c3bfd8e5660f4537`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684dd6070aa89f7d64e27f891d77a5fea632b893241ff66da06f16e54b3c96a6`  
		Last Modified: Thu, 21 Jan 2021 04:42:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c67edb3d568d86357a630edc1923d8fa70e3eea8bc5920edcf29dab66f11d4`  
		Last Modified: Thu, 21 Jan 2021 04:42:22 GMT  
		Size: 139.3 MB (139273378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e1ffd4eb011cb4d1416bf7f49751b13a4dfb5b0c37238e672290617b87dcf4`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efad1d47d721328a8ba57a39bc62b6560d33378f004345c4e3b5c39baf6fd48`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:c411bd2e1a16b2ed7137b3f4dde84bf8f4c920369bf4498fe3d0841e70388434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:4-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a218b70c050ffcd70e88e2969459b0b990e9e0f4e32973a5e090ab7785ab7bcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:84704a0ba708c7ebe301eefad6f553d9eae46c1640dc29371dc211f22589cc99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:0290400e988ee9856ad321f81781827e0124d13f68cc72d6cad4807f3174946c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:06ba42906e0346c15a795ff6ebcb3ac88be0f85aa899a6225979029188e312c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178222610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8e14b1fda68aedb435fec2a6eaa326cf5633fc57b7e28b5cc37d938ead9edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:23:24 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 10:23:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:26 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 10:23:28 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:52 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:52 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca70046d298d7aac215eecead78d18f8f28e11eaea6db7f35c945e64a43124`  
		Last Modified: Thu, 21 Jan 2021 10:25:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a541da2a89089f196a998312c16f37f8ee11251f88d764ce95274dd29d5a3`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18edd0c32639b9f81da45ecc082e23f67c7eb02bc3a1216622dfe181c852f505`  
		Last Modified: Thu, 21 Jan 2021 10:26:20 GMT  
		Size: 142.7 MB (142686014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86830e28cf719e7b6459badd7a5ade676e32d9b08c004774f65dce25bc639636`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1d772417d960c2608d622279c356232f0b70a0b82c7129bf57df7f4c1aeea`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:35d866a5fd70ff9b9cd520ad48bc4250f1a4e05171b205fcfc68fe9c51efa8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168151561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095aea9826c2c421ae2b1c4299766ba6461174f3a901019cb427b1d1cf54f5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:55:16 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 05:55:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:55:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:55:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:21 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 05:55:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:55:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:55:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:55:55 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:55:56 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:57 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:55:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f46ba3c06d737a4d0e64c1f3db503400ee0eb1b4b4bb586b0bd7f9ded60c3a`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144bd8644f0fbdd12fa8e9850c9036f763fb7720a1a580a0ad88bd9c35fc4684`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250692aff7a7255ff3544fd94c39f0a2896636ced434869481c1029047068c4`  
		Last Modified: Thu, 21 Jan 2021 05:58:51 GMT  
		Size: 136.4 MB (136380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f467e359b3608c8a4425b25553555612e50e64f8e954c382195fcf3cd28401d0`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a524c0aa3acb289bb84a7514ddf6c6ac6cb5feb52a04d253aedc50de4a73488e`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:9c0b379fa79bc55520a9badaf4ac04a213d55e2e76c1f453261e7010e62c1b82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173132528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc71b87dda565765e825ef3f366cd24b6512c3c1495ee26e640d82412d9ed5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 04:00:45 GMT
ADD file:d443bbf06b974365e3cb2d99eea08d454059cf95b82a6023e4260fba5ead568e in / 
# Thu, 21 Jan 2021 04:00:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:00:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:00:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:00:56 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 04:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:39:49 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 04:39:50 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 04:40:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 04:40:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 04:40:15 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 04:40:17 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 04:40:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 04:41:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 04:41:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 04:41:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 04:41:25 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 04:41:27 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 04:41:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1a4e1c3f599543fe1043f321c3c5e14f5ca6073cba211f2144b569c5d0cff014`  
		Last Modified: Thu, 21 Jan 2021 04:03:17 GMT  
		Size: 25.4 MB (25381801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1202f2791a7390dbd7197d4cfde724e184be1b2f9d4791890fb64341336f889e`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c44bad24828f92a8ff703d4d356f2969f0c1de9f6d852d3cec338a3aff6265`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad237e33328657490128a3945e880b746ebd50c75cc14cb7e6cb1e2c60e8a1b`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2023f0f19357e97e77398f90b92a5736e2f71e3413a2fdc91330fc05461250`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 2.7 MB (2721180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb06349457fa157b55404be7a301c14dce1915009bad7fa29e12925d5821993`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 5.7 MB (5746846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33428088ab5395067d4b3d3b8dee47ab7f7237cdd0a4df0e3f6b8521c3fb839b`  
		Last Modified: Thu, 21 Jan 2021 04:42:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3464b0455ffb640246507864b1476076c6d50b7235fbc64c3bfd8e5660f4537`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684dd6070aa89f7d64e27f891d77a5fea632b893241ff66da06f16e54b3c96a6`  
		Last Modified: Thu, 21 Jan 2021 04:42:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c67edb3d568d86357a630edc1923d8fa70e3eea8bc5920edcf29dab66f11d4`  
		Last Modified: Thu, 21 Jan 2021 04:42:22 GMT  
		Size: 139.3 MB (139273378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e1ffd4eb011cb4d1416bf7f49751b13a4dfb5b0c37238e672290617b87dcf4`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efad1d47d721328a8ba57a39bc62b6560d33378f004345c4e3b5c39baf6fd48`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:88e0308671a06d4ee7da41f87944ba66355b4ee3d57d57caf92f5e1938736abd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:06ba42906e0346c15a795ff6ebcb3ac88be0f85aa899a6225979029188e312c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178222610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8e14b1fda68aedb435fec2a6eaa326cf5633fc57b7e28b5cc37d938ead9edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:22:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 10:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:22:40 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 10:22:40 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 10:22:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 10:22:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 10:23:24 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 10:23:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 10:23:26 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:26 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 10:23:27 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 10:23:28 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 10:23:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 10:23:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 10:23:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 10:23:52 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 10:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:23:52 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 10:23:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c1234bf134339f590a033b18bddfb9ec33c7ca2c31142922a842e10e4cfb25`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf57f3b398e4e62a9cc63cbe5c4451ec8a516f397f174d59c4b4c47d80ab72`  
		Last Modified: Thu, 21 Jan 2021 10:25:32 GMT  
		Size: 3.0 MB (2990876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737ab85f84cf15c6c08486c43ad3846cb58ddda63aeb94e95b344d18e59d46c`  
		Last Modified: Thu, 21 Jan 2021 10:25:34 GMT  
		Size: 5.8 MB (5826781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6165557c172c38bcf7ac779522be7ed1f0176f56e20b594ad7246cf1e84b9a7a`  
		Last Modified: Thu, 21 Jan 2021 10:25:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca70046d298d7aac215eecead78d18f8f28e11eaea6db7f35c945e64a43124`  
		Last Modified: Thu, 21 Jan 2021 10:25:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a541da2a89089f196a998312c16f37f8ee11251f88d764ce95274dd29d5a3`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18edd0c32639b9f81da45ecc082e23f67c7eb02bc3a1216622dfe181c852f505`  
		Last Modified: Thu, 21 Jan 2021 10:26:20 GMT  
		Size: 142.7 MB (142686014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86830e28cf719e7b6459badd7a5ade676e32d9b08c004774f65dce25bc639636`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1d772417d960c2608d622279c356232f0b70a0b82c7129bf57df7f4c1aeea`  
		Last Modified: Thu, 21 Jan 2021 10:25:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:35d866a5fd70ff9b9cd520ad48bc4250f1a4e05171b205fcfc68fe9c51efa8e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168151561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095aea9826c2c421ae2b1c4299766ba6461174f3a901019cb427b1d1cf54f5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:53:44 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 05:54:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:01 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:54:01 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 05:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:54:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:55:16 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 05:55:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:55:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 05:55:20 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:21 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 05:55:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 05:55:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 05:55:51 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 05:55:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 05:55:55 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 05:55:56 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:57 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 05:55:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43d4fc6b57df76539ecc3bb13ce754ca842358014f1dddbc8ddba4b66c5a588`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e242f03c2ade0d30a8a4b10ba09bf92e5c63fc602db6dfa4eca1658d694daea`  
		Last Modified: Thu, 21 Jan 2021 05:57:44 GMT  
		Size: 2.7 MB (2681995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8609d4097ab98b95005c224b84e39606fa73cb4dddc4883790e3edb70d4fac70`  
		Last Modified: Thu, 21 Jan 2021 05:57:45 GMT  
		Size: 5.3 MB (5346733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8876bad2c8ce97582b86e9f352dc4688656437d72a69bdaeca26ead0b96cb1ea`  
		Last Modified: Thu, 21 Jan 2021 05:57:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f46ba3c06d737a4d0e64c1f3db503400ee0eb1b4b4bb586b0bd7f9ded60c3a`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144bd8644f0fbdd12fa8e9850c9036f763fb7720a1a580a0ad88bd9c35fc4684`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250692aff7a7255ff3544fd94c39f0a2896636ced434869481c1029047068c4`  
		Last Modified: Thu, 21 Jan 2021 05:58:51 GMT  
		Size: 136.4 MB (136380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f467e359b3608c8a4425b25553555612e50e64f8e954c382195fcf3cd28401d0`  
		Last Modified: Thu, 21 Jan 2021 05:58:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a524c0aa3acb289bb84a7514ddf6c6ac6cb5feb52a04d253aedc50de4a73488e`  
		Last Modified: Thu, 21 Jan 2021 05:58:19 GMT  
		Size: 4.4 KB (4418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:9c0b379fa79bc55520a9badaf4ac04a213d55e2e76c1f453261e7010e62c1b82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173132528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc71b87dda565765e825ef3f366cd24b6512c3c1495ee26e640d82412d9ed5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 21 Jan 2021 04:00:45 GMT
ADD file:d443bbf06b974365e3cb2d99eea08d454059cf95b82a6023e4260fba5ead568e in / 
# Thu, 21 Jan 2021 04:00:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:00:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:00:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:00:56 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 21 Jan 2021 04:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:39:49 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 04:39:50 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 21 Jan 2021 04:40:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 04:40:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 04:40:15 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 21 Jan 2021 04:40:17 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Jan 2021 04:40:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_MAJOR=4.4
# Thu, 21 Jan 2021 04:40:20 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 21 Jan 2021 04:40:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Jan 2021 04:41:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Jan 2021 04:41:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Jan 2021 04:41:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Jan 2021 04:41:25 GMT
COPY file:5099dacbd8c203daf370fa53aaec9cf565b8b25f3c697b59e68ecb6c9499e360 in /usr/local/bin/ 
# Thu, 21 Jan 2021 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 04:41:27 GMT
EXPOSE 27017
# Thu, 21 Jan 2021 04:41:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:1a4e1c3f599543fe1043f321c3c5e14f5ca6073cba211f2144b569c5d0cff014`  
		Last Modified: Thu, 21 Jan 2021 04:03:17 GMT  
		Size: 25.4 MB (25381801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1202f2791a7390dbd7197d4cfde724e184be1b2f9d4791890fb64341336f889e`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c44bad24828f92a8ff703d4d356f2969f0c1de9f6d852d3cec338a3aff6265`  
		Last Modified: Thu, 21 Jan 2021 04:03:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad237e33328657490128a3945e880b746ebd50c75cc14cb7e6cb1e2c60e8a1b`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2023f0f19357e97e77398f90b92a5736e2f71e3413a2fdc91330fc05461250`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 2.7 MB (2721180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb06349457fa157b55404be7a301c14dce1915009bad7fa29e12925d5821993`  
		Last Modified: Thu, 21 Jan 2021 04:42:06 GMT  
		Size: 5.7 MB (5746846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33428088ab5395067d4b3d3b8dee47ab7f7237cdd0a4df0e3f6b8521c3fb839b`  
		Last Modified: Thu, 21 Jan 2021 04:42:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3464b0455ffb640246507864b1476076c6d50b7235fbc64c3bfd8e5660f4537`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684dd6070aa89f7d64e27f891d77a5fea632b893241ff66da06f16e54b3c96a6`  
		Last Modified: Thu, 21 Jan 2021 04:42:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c67edb3d568d86357a630edc1923d8fa70e3eea8bc5920edcf29dab66f11d4`  
		Last Modified: Thu, 21 Jan 2021 04:42:22 GMT  
		Size: 139.3 MB (139273378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e1ffd4eb011cb4d1416bf7f49751b13a4dfb5b0c37238e672290617b87dcf4`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efad1d47d721328a8ba57a39bc62b6560d33378f004345c4e3b5c39baf6fd48`  
		Last Modified: Thu, 21 Jan 2021 04:42:02 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:c411bd2e1a16b2ed7137b3f4dde84bf8f4c920369bf4498fe3d0841e70388434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `mongo:windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:a218b70c050ffcd70e88e2969459b0b990e9e0f4e32973a5e090ab7785ab7bcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:84704a0ba708c7ebe301eefad6f553d9eae46c1640dc29371dc211f22589cc99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:d898e4ee7db840baa82afab91bf427c07498b9655dbe50a5869f70a9c62b74aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6034607102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1937b9937c2570d1bb587fe797fe2157748b6c9a384d4ca16b88dbea0e787295`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:52:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:52:07 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:56:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:56:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:56:11 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:56:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a56f5bbb5d29b5616f3447e484fe49c7fa35c547b6c62d525a30f57f5a82bc`  
		Last Modified: Thu, 14 Jan 2021 01:12:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593aa0243f57624b277e407618df858a817ec5fcb0b505458ddf004bc03bce2`  
		Last Modified: Thu, 14 Jan 2021 01:12:53 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3af304ffeca3c91850737fba9fd54aa8359094a67e983dc9feead1f895f4e7`  
		Last Modified: Thu, 14 Jan 2021 01:12:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65024d914edc56351197da8cc65ae3959cd2432b771bd555f066b9f9e2f937b6`  
		Last Modified: Thu, 14 Jan 2021 01:13:35 GMT  
		Size: 240.7 MB (240705044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67ad03c84f732669ccf9fb571c9b83276c59f0c39aeb85a2fc559f5c5466f49`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbf4a797ee6109ac7b03f41f7d0a76482f8a75aa4b9158e695bbd5d6f8990`  
		Last Modified: Thu, 14 Jan 2021 01:12:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c57dc16aa26db1b79843afabfae90b3b681b240beb9cfb45f2a1f6dc75da6`  
		Last Modified: Thu, 14 Jan 2021 01:12:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
