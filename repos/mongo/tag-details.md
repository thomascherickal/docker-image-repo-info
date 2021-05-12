<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3-windowsservercore`](#mongo3-windowsservercore)
-	[`mongo:3-windowsservercore-1809`](#mongo3-windowsservercore-1809)
-	[`mongo:3-windowsservercore-ltsc2016`](#mongo3-windowsservercore-ltsc2016)
-	[`mongo:3-xenial`](#mongo3-xenial)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6-windowsservercore`](#mongo36-windowsservercore)
-	[`mongo:3.6-windowsservercore-1809`](#mongo36-windowsservercore-1809)
-	[`mongo:3.6-windowsservercore-ltsc2016`](#mongo36-windowsservercore-ltsc2016)
-	[`mongo:3.6-xenial`](#mongo36-xenial)
-	[`mongo:3.6.23`](#mongo3623)
-	[`mongo:3.6.23-windowsservercore`](#mongo3623-windowsservercore)
-	[`mongo:3.6.23-windowsservercore-1809`](#mongo3623-windowsservercore-1809)
-	[`mongo:3.6.23-windowsservercore-ltsc2016`](#mongo3623-windowsservercore-ltsc2016)
-	[`mongo:3.6.23-xenial`](#mongo3623-xenial)
-	[`mongo:4`](#mongo4)
-	[`mongo:4-bionic`](#mongo4-bionic)
-	[`mongo:4-windowsservercore`](#mongo4-windowsservercore)
-	[`mongo:4-windowsservercore-1809`](#mongo4-windowsservercore-1809)
-	[`mongo:4-windowsservercore-ltsc2016`](#mongo4-windowsservercore-ltsc2016)
-	[`mongo:4.0`](#mongo40)
-	[`mongo:4.0-windowsservercore`](#mongo40-windowsservercore)
-	[`mongo:4.0-windowsservercore-1809`](#mongo40-windowsservercore-1809)
-	[`mongo:4.0-windowsservercore-ltsc2016`](#mongo40-windowsservercore-ltsc2016)
-	[`mongo:4.0-xenial`](#mongo40-xenial)
-	[`mongo:4.0.24`](#mongo4024)
-	[`mongo:4.0.24-windowsservercore`](#mongo4024-windowsservercore)
-	[`mongo:4.0.24-windowsservercore-1809`](#mongo4024-windowsservercore-1809)
-	[`mongo:4.0.24-windowsservercore-ltsc2016`](#mongo4024-windowsservercore-ltsc2016)
-	[`mongo:4.0.24-xenial`](#mongo4024-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2-bionic`](#mongo42-bionic)
-	[`mongo:4.2-windowsservercore`](#mongo42-windowsservercore)
-	[`mongo:4.2-windowsservercore-1809`](#mongo42-windowsservercore-1809)
-	[`mongo:4.2-windowsservercore-ltsc2016`](#mongo42-windowsservercore-ltsc2016)
-	[`mongo:4.2.14`](#mongo4214)
-	[`mongo:4.2.14-bionic`](#mongo4214-bionic)
-	[`mongo:4.2.14-windowsservercore`](#mongo4214-windowsservercore)
-	[`mongo:4.2.14-windowsservercore-1809`](#mongo4214-windowsservercore-1809)
-	[`mongo:4.2.14-windowsservercore-ltsc2016`](#mongo4214-windowsservercore-ltsc2016)
-	[`mongo:4.4`](#mongo44)
-	[`mongo:4.4-bionic`](#mongo44-bionic)
-	[`mongo:4.4-windowsservercore`](#mongo44-windowsservercore)
-	[`mongo:4.4-windowsservercore-1809`](#mongo44-windowsservercore-1809)
-	[`mongo:4.4-windowsservercore-ltsc2016`](#mongo44-windowsservercore-ltsc2016)
-	[`mongo:4.4.6`](#mongo446)
-	[`mongo:4.4.6-bionic`](#mongo446-bionic)
-	[`mongo:4.4.6-windowsservercore`](#mongo446-windowsservercore)
-	[`mongo:4.4.6-windowsservercore-1809`](#mongo446-windowsservercore-1809)
-	[`mongo:4.4.6-windowsservercore-ltsc2016`](#mongo446-windowsservercore-ltsc2016)
-	[`mongo:bionic`](#mongobionic)
-	[`mongo:latest`](#mongolatest)
-	[`mongo:windowsservercore`](#mongowindowsservercore)
-	[`mongo:windowsservercore-1809`](#mongowindowsservercore-1809)
-	[`mongo:windowsservercore-ltsc2016`](#mongowindowsservercore-ltsc2016)

## `mongo:3`

```console
$ docker pull mongo@sha256:146c1fd999a660e697aac40bc6da842b005c7868232eb0b7d8996c8f3545b05d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:19c11a8f1064fd2bb713ef1270f79a742a184cd57d9bb922efdd2a8eca514af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.9 MB (169884275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f21415cb85f27d2069174ca001af3c0ebb95a5b3c3520bf59af30395481deb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:14 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 00:40:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 00:40:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:40:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:40:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:40:35 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:14 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:15 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2928038a60539dc0be050a03515200578116a63feb1a7cb2fea42f22ff015b15`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a16c1b79ab70d832c5a48c0122d9391279714757b1fcbd41b6d2b82e1ee0d8`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec0f86077cfba84fc9ba3266319f50145c59a883f62b2fa73250ef81670078`  
		Last Modified: Sat, 24 Apr 2021 00:43:06 GMT  
		Size: 119.4 MB (119407719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261a04726d31c63ac3df481d8d1388b33dc13c45b29059901728368f3b16be5b`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4062426e720d589a9b63fb138f0198937bf230b1371b4ded281368d28d40c8`  
		Last Modified: Thu, 06 May 2021 23:35:54 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f9b01e368fd95a783a68471930a15c2494d525318ff65a1b408ff3e6bc83e3d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158083060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c00894eae7a1ee8beaa4bdd19711ee336744f3ff75af4ef92d98fd74e9f72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:48:08 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 01:48:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:48:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:48:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 01:48:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:48:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:48:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:48:56 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:34 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:37 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:38 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314de618082ca7596a3ec4a34670c242bada578c9f5e9ee3ebf2dc6a58f30066`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c764d07a252bab6a0202f60b5d24a8b7d9ef68860bb05855911409a1c057d4`  
		Last Modified: Sat, 24 Apr 2021 01:54:24 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5923a419767af92edb639be1fc8a41b15bab4093b3431f56590dd46e3b1d469e`  
		Last Modified: Sat, 24 Apr 2021 01:54:49 GMT  
		Size: 113.4 MB (113379478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d422d31688243ab9fb74c0f065d222ecc9bf8c2e1faf94156df93a7a599bccc7`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028ad5b7f9fb5f7da5701db59aa7005cca4935029ce3839d3f090b681358e678`  
		Last Modified: Fri, 07 May 2021 01:19:39 GMT  
		Size: 4.5 KB (4472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:7b251c9082a6f50344bc4d628780e099faf0da03a813487b6fcbcb375ea5cdc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:3-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:19b27b98218b2bda1fcb7008b2c9570f477a578207f918d6281bac49f0d55e59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:2418d05e46e249c4dc6592f7214afaf9f854fc00a41ed507340c13e13a69ccd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:e8c30352bb2ff2fbe886771085af52276c053eee9eaf57194a1facfb695b760e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:19c11a8f1064fd2bb713ef1270f79a742a184cd57d9bb922efdd2a8eca514af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.9 MB (169884275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f21415cb85f27d2069174ca001af3c0ebb95a5b3c3520bf59af30395481deb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:14 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 00:40:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 00:40:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:40:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:40:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:40:35 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:14 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:15 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2928038a60539dc0be050a03515200578116a63feb1a7cb2fea42f22ff015b15`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a16c1b79ab70d832c5a48c0122d9391279714757b1fcbd41b6d2b82e1ee0d8`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec0f86077cfba84fc9ba3266319f50145c59a883f62b2fa73250ef81670078`  
		Last Modified: Sat, 24 Apr 2021 00:43:06 GMT  
		Size: 119.4 MB (119407719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261a04726d31c63ac3df481d8d1388b33dc13c45b29059901728368f3b16be5b`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4062426e720d589a9b63fb138f0198937bf230b1371b4ded281368d28d40c8`  
		Last Modified: Thu, 06 May 2021 23:35:54 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f9b01e368fd95a783a68471930a15c2494d525318ff65a1b408ff3e6bc83e3d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158083060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c00894eae7a1ee8beaa4bdd19711ee336744f3ff75af4ef92d98fd74e9f72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:48:08 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 01:48:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:48:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:48:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 01:48:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:48:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:48:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:48:56 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:34 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:37 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:38 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314de618082ca7596a3ec4a34670c242bada578c9f5e9ee3ebf2dc6a58f30066`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c764d07a252bab6a0202f60b5d24a8b7d9ef68860bb05855911409a1c057d4`  
		Last Modified: Sat, 24 Apr 2021 01:54:24 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5923a419767af92edb639be1fc8a41b15bab4093b3431f56590dd46e3b1d469e`  
		Last Modified: Sat, 24 Apr 2021 01:54:49 GMT  
		Size: 113.4 MB (113379478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d422d31688243ab9fb74c0f065d222ecc9bf8c2e1faf94156df93a7a599bccc7`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028ad5b7f9fb5f7da5701db59aa7005cca4935029ce3839d3f090b681358e678`  
		Last Modified: Fri, 07 May 2021 01:19:39 GMT  
		Size: 4.5 KB (4472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:146c1fd999a660e697aac40bc6da842b005c7868232eb0b7d8996c8f3545b05d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:19c11a8f1064fd2bb713ef1270f79a742a184cd57d9bb922efdd2a8eca514af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.9 MB (169884275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f21415cb85f27d2069174ca001af3c0ebb95a5b3c3520bf59af30395481deb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:14 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 00:40:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 00:40:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:40:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:40:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:40:35 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:14 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:15 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2928038a60539dc0be050a03515200578116a63feb1a7cb2fea42f22ff015b15`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a16c1b79ab70d832c5a48c0122d9391279714757b1fcbd41b6d2b82e1ee0d8`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec0f86077cfba84fc9ba3266319f50145c59a883f62b2fa73250ef81670078`  
		Last Modified: Sat, 24 Apr 2021 00:43:06 GMT  
		Size: 119.4 MB (119407719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261a04726d31c63ac3df481d8d1388b33dc13c45b29059901728368f3b16be5b`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4062426e720d589a9b63fb138f0198937bf230b1371b4ded281368d28d40c8`  
		Last Modified: Thu, 06 May 2021 23:35:54 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f9b01e368fd95a783a68471930a15c2494d525318ff65a1b408ff3e6bc83e3d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158083060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c00894eae7a1ee8beaa4bdd19711ee336744f3ff75af4ef92d98fd74e9f72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:48:08 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 01:48:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:48:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:48:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 01:48:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:48:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:48:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:48:56 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:34 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:37 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:38 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314de618082ca7596a3ec4a34670c242bada578c9f5e9ee3ebf2dc6a58f30066`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c764d07a252bab6a0202f60b5d24a8b7d9ef68860bb05855911409a1c057d4`  
		Last Modified: Sat, 24 Apr 2021 01:54:24 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5923a419767af92edb639be1fc8a41b15bab4093b3431f56590dd46e3b1d469e`  
		Last Modified: Sat, 24 Apr 2021 01:54:49 GMT  
		Size: 113.4 MB (113379478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d422d31688243ab9fb74c0f065d222ecc9bf8c2e1faf94156df93a7a599bccc7`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028ad5b7f9fb5f7da5701db59aa7005cca4935029ce3839d3f090b681358e678`  
		Last Modified: Fri, 07 May 2021 01:19:39 GMT  
		Size: 4.5 KB (4472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:7b251c9082a6f50344bc4d628780e099faf0da03a813487b6fcbcb375ea5cdc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:19b27b98218b2bda1fcb7008b2c9570f477a578207f918d6281bac49f0d55e59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:2418d05e46e249c4dc6592f7214afaf9f854fc00a41ed507340c13e13a69ccd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:e8c30352bb2ff2fbe886771085af52276c053eee9eaf57194a1facfb695b760e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:19c11a8f1064fd2bb713ef1270f79a742a184cd57d9bb922efdd2a8eca514af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.9 MB (169884275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f21415cb85f27d2069174ca001af3c0ebb95a5b3c3520bf59af30395481deb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:14 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 00:40:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 00:40:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:40:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:40:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:40:35 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:14 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:15 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2928038a60539dc0be050a03515200578116a63feb1a7cb2fea42f22ff015b15`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a16c1b79ab70d832c5a48c0122d9391279714757b1fcbd41b6d2b82e1ee0d8`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec0f86077cfba84fc9ba3266319f50145c59a883f62b2fa73250ef81670078`  
		Last Modified: Sat, 24 Apr 2021 00:43:06 GMT  
		Size: 119.4 MB (119407719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261a04726d31c63ac3df481d8d1388b33dc13c45b29059901728368f3b16be5b`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4062426e720d589a9b63fb138f0198937bf230b1371b4ded281368d28d40c8`  
		Last Modified: Thu, 06 May 2021 23:35:54 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f9b01e368fd95a783a68471930a15c2494d525318ff65a1b408ff3e6bc83e3d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158083060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c00894eae7a1ee8beaa4bdd19711ee336744f3ff75af4ef92d98fd74e9f72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:48:08 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 01:48:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:48:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:48:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 01:48:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:48:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:48:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:48:56 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:34 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:37 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:38 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314de618082ca7596a3ec4a34670c242bada578c9f5e9ee3ebf2dc6a58f30066`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c764d07a252bab6a0202f60b5d24a8b7d9ef68860bb05855911409a1c057d4`  
		Last Modified: Sat, 24 Apr 2021 01:54:24 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5923a419767af92edb639be1fc8a41b15bab4093b3431f56590dd46e3b1d469e`  
		Last Modified: Sat, 24 Apr 2021 01:54:49 GMT  
		Size: 113.4 MB (113379478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d422d31688243ab9fb74c0f065d222ecc9bf8c2e1faf94156df93a7a599bccc7`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028ad5b7f9fb5f7da5701db59aa7005cca4935029ce3839d3f090b681358e678`  
		Last Modified: Fri, 07 May 2021 01:19:39 GMT  
		Size: 4.5 KB (4472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23`

```console
$ docker pull mongo@sha256:146c1fd999a660e697aac40bc6da842b005c7868232eb0b7d8996c8f3545b05d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:3.6.23` - linux; amd64

```console
$ docker pull mongo@sha256:19c11a8f1064fd2bb713ef1270f79a742a184cd57d9bb922efdd2a8eca514af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.9 MB (169884275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f21415cb85f27d2069174ca001af3c0ebb95a5b3c3520bf59af30395481deb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:14 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 00:40:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 00:40:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:40:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:40:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:40:35 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:14 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:15 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2928038a60539dc0be050a03515200578116a63feb1a7cb2fea42f22ff015b15`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a16c1b79ab70d832c5a48c0122d9391279714757b1fcbd41b6d2b82e1ee0d8`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec0f86077cfba84fc9ba3266319f50145c59a883f62b2fa73250ef81670078`  
		Last Modified: Sat, 24 Apr 2021 00:43:06 GMT  
		Size: 119.4 MB (119407719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261a04726d31c63ac3df481d8d1388b33dc13c45b29059901728368f3b16be5b`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4062426e720d589a9b63fb138f0198937bf230b1371b4ded281368d28d40c8`  
		Last Modified: Thu, 06 May 2021 23:35:54 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f9b01e368fd95a783a68471930a15c2494d525318ff65a1b408ff3e6bc83e3d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158083060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c00894eae7a1ee8beaa4bdd19711ee336744f3ff75af4ef92d98fd74e9f72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:48:08 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 01:48:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:48:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:48:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 01:48:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:48:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:48:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:48:56 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:34 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:37 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:38 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314de618082ca7596a3ec4a34670c242bada578c9f5e9ee3ebf2dc6a58f30066`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c764d07a252bab6a0202f60b5d24a8b7d9ef68860bb05855911409a1c057d4`  
		Last Modified: Sat, 24 Apr 2021 01:54:24 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5923a419767af92edb639be1fc8a41b15bab4093b3431f56590dd46e3b1d469e`  
		Last Modified: Sat, 24 Apr 2021 01:54:49 GMT  
		Size: 113.4 MB (113379478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d422d31688243ab9fb74c0f065d222ecc9bf8c2e1faf94156df93a7a599bccc7`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028ad5b7f9fb5f7da5701db59aa7005cca4935029ce3839d3f090b681358e678`  
		Last Modified: Fri, 07 May 2021 01:19:39 GMT  
		Size: 4.5 KB (4472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23-windowsservercore`

```console
$ docker pull mongo@sha256:7b251c9082a6f50344bc4d628780e099faf0da03a813487b6fcbcb375ea5cdc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:3.6.23-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23-windowsservercore-1809`

```console
$ docker pull mongo@sha256:19b27b98218b2bda1fcb7008b2c9570f477a578207f918d6281bac49f0d55e59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:3.6.23-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:bbb44a208559a1fad8f164e0bd97db2b9f4b699d6adfa01ba4f20b9ec60eb832
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700890096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec03f5b56d213beb494f669ff8eab06c415caa4da8c072dfab81373a6b30d480`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:54:14 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:54:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:54:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Tue, 11 May 2021 23:58:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 11 May 2021 23:58:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 11 May 2021 23:58:16 GMT
EXPOSE 27017
# Tue, 11 May 2021 23:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43e506c53440ad09d8e3d8d28da0572bdb5fb2585cff7c32f9150add8a2d9d`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266d67fce156b20492d637ca414bcf724c7c49b5f51aeecefe126d091c474053`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6412b8dff95bf66f633f13fcacc76cfc3792bfa527af4a705fe43ad2c5b9a49`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29c27943a96936fd7f9f3db2e7cd0a6b04b4d090e6be3e420237e61ea940b8`  
		Last Modified: Wed, 12 May 2021 00:46:06 GMT  
		Size: 226.4 MB (226390889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574d631beb757810238376cdfe620f7d6d1d9412711548bd6976b291889c138`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdf8df467b8ff7dfa85c3749b3e3a302c6db5957be67cb313dd7dc9d371b6ae`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb35e6510407cbcbe7cb2b4edbf6ba2eadc69c3245b38b88cd432394c86c88`  
		Last Modified: Wed, 12 May 2021 00:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:2418d05e46e249c4dc6592f7214afaf9f854fc00a41ed507340c13e13a69ccd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:3.6.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:bc25ab206f79c4618ca23b8fb5f8b2710783ed6a5058f30e8f196a85f3f5c3fb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6027234545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f815a1443565a889d7c545055a5a29a8fe915c09eb90e29c52fc1bffb19d19`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 May 2021 23:58:34 GMT
ENV MONGO_VERSION=3.6.23
# Tue, 11 May 2021 23:58:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Tue, 11 May 2021 23:58:37 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Wed, 12 May 2021 00:02:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:02:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:02:52 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:02:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c5d1b769ad56f554cfdc9054daac0721d63847b03ba62f4a17c23cdfbf3c8`  
		Last Modified: Wed, 12 May 2021 00:46:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f43a73bd273da7241a2f64cb84499c09b0ad3d8dd4ce5b851e218e6fcb8472`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836f67bccbeea6d12c908fc5e144a71010a49dbfd2071d46a2a06f9ebbdb7f0`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fa3ead545ee758764b89edc5be38cea416a1077955eae832ccd07a9a03126f`  
		Last Modified: Wed, 12 May 2021 00:47:43 GMT  
		Size: 231.4 MB (231447233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937272dbd650948962febfb036ef9dad8bf8dbb2d32555a076aa55ebef6bd6d`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81698c4f9c159f4ffcdb5cc1ce672406ae0d687b2128e3b9c1aab3d18c7cc97`  
		Last Modified: Wed, 12 May 2021 00:46:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d3078b1b4da7eaf5e95d1d6a3aed9be85d236da0320cf91fca513793acf8fb`  
		Last Modified: Wed, 12 May 2021 00:46:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23-xenial`

```console
$ docker pull mongo@sha256:e8c30352bb2ff2fbe886771085af52276c053eee9eaf57194a1facfb695b760e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.23-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:19c11a8f1064fd2bb713ef1270f79a742a184cd57d9bb922efdd2a8eca514af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.9 MB (169884275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f21415cb85f27d2069174ca001af3c0ebb95a5b3c3520bf59af30395481deb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:14 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 00:40:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:16 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 00:40:16 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 00:40:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:40:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:40:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:40:35 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:14 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:15 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2928038a60539dc0be050a03515200578116a63feb1a7cb2fea42f22ff015b15`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a16c1b79ab70d832c5a48c0122d9391279714757b1fcbd41b6d2b82e1ee0d8`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec0f86077cfba84fc9ba3266319f50145c59a883f62b2fa73250ef81670078`  
		Last Modified: Sat, 24 Apr 2021 00:43:06 GMT  
		Size: 119.4 MB (119407719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261a04726d31c63ac3df481d8d1388b33dc13c45b29059901728368f3b16be5b`  
		Last Modified: Sat, 24 Apr 2021 00:42:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4062426e720d589a9b63fb138f0198937bf230b1371b4ded281368d28d40c8`  
		Last Modified: Thu, 06 May 2021 23:35:54 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f9b01e368fd95a783a68471930a15c2494d525318ff65a1b408ff3e6bc83e3d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158083060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c00894eae7a1ee8beaa4bdd19711ee336744f3ff75af4ef92d98fd74e9f72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:48:08 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 24 Apr 2021 01:48:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:48:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:48:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_MAJOR=3.6
# Sat, 24 Apr 2021 01:48:14 GMT
ENV MONGO_VERSION=3.6.23
# Sat, 24 Apr 2021 01:48:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:48:50 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:48:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:48:56 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:34 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:37 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:38 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314de618082ca7596a3ec4a34670c242bada578c9f5e9ee3ebf2dc6a58f30066`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c764d07a252bab6a0202f60b5d24a8b7d9ef68860bb05855911409a1c057d4`  
		Last Modified: Sat, 24 Apr 2021 01:54:24 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5923a419767af92edb639be1fc8a41b15bab4093b3431f56590dd46e3b1d469e`  
		Last Modified: Sat, 24 Apr 2021 01:54:49 GMT  
		Size: 113.4 MB (113379478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d422d31688243ab9fb74c0f065d222ecc9bf8c2e1faf94156df93a7a599bccc7`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028ad5b7f9fb5f7da5701db59aa7005cca4935029ce3839d3f090b681358e678`  
		Last Modified: Fri, 07 May 2021 01:19:39 GMT  
		Size: 4.5 KB (4472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:401ae88210c708d54873af22df618b46a5f3d2da1c2676d115326b205ec78d3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:ebb6b8403c1f47069b099f1ba75778d41e15a5d8eed3db6f435733333e403a2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175677269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07630e791de3ceb87d39543799438e118753246d19dcfd6529bd4d27ff1b83bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:58 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 00:41:59 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:11:00 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:11:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:11:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:11:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:11:48 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:11:49 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:11:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:11:49 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:11:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2ff17242ce7e307fbd191a597f210061566606443ff6632ca685d394cb9acf`  
		Last Modified: Sat, 24 Apr 2021 00:44:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11b2ce05942f19ca819aa8c130575b0850153384fba7f489fd1a62ec0d94e7`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91532386f4ec7af743bc43ddbab8410d9d2fee68ce63bca3aa397c04e29b9091`  
		Last Modified: Tue, 11 May 2021 00:12:51 GMT  
		Size: 140.2 MB (140162019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705ef0ab262e766f32008195b4e3719f5444b83e3218dbab09f5cfa7098322ea`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6238126b609f01bb47ddd8598f331bb5cb7653f2d9798eb2f14d48061d8e279`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 4.5 KB (4477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8f2c9016beb50c2972e54c732d8dc24fb332360104b9e71767af9c4e71c1348e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168070890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3a757873434f9961cb2b732f35c712866d65e5fdf009c9b8572d46c0657e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 01:53:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:53:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:08 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 01:41:03 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 01:41:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 01:41:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 01:41:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 01:41:41 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 01:41:42 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 01:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:41:44 GMT
EXPOSE 27017
# Tue, 11 May 2021 01:41:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b8f707197ef2788f2ed0cf82b088b9262efb9b7a374da64bb70daccca6525`  
		Last Modified: Sat, 24 Apr 2021 01:56:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d9f84ef7c607013458b7c4f0045d42081a3cd4e32e09a99c45af7af1742eb`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a71fa0bced6eaef2a94dfda7f28a3c97b1f52e0def1e877932edf84e97df5`  
		Last Modified: Tue, 11 May 2021 01:42:41 GMT  
		Size: 136.3 MB (136341433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88698b947abf4aa832fdbc0c629195e7b8ad1790baad6dfa6ad42b0201e5b81e`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7dfc922696b1eae0c53f3c4559bdfca5ae0dd740a6c3e5166c0839e4ce49ad`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:c8e981f281462baf0c84890eab82c4fad6c825d221664b463ccd43485f6380cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169474559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8b1f024425214a141ef62568a875dc3f443453094dbe43757c3a42d5ada69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:51:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Apr 2021 22:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:51:56 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 22:51:57 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Apr 2021 22:52:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 22:52:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 22:52:19 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 23 Apr 2021 22:52:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:24 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:38:53 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:38:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:39:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:39:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:39:55 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:39:55 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:39:56 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:39:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bc20f34c3c0e6defa11123a46488ad9866f1cbed77d74904f7b057f014902`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934bd72760b936ef87cda05b4fd31a1266859e77f6960e8b6a17eb4df55b82b2`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 2.7 MB (2708330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778576254d798d87ee503dd46947744945440e160227cf20f86506eb7f0c752`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 5.7 MB (5747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b7218def3876e2bd7ede8db669dd67c94e3f67db5c8b385e7d0b189c70f19`  
		Last Modified: Fri, 23 Apr 2021 22:53:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218c55b05ae6da8d768db66caf009228dd32c56943df536e02932cd24a359f1e`  
		Last Modified: Fri, 23 Apr 2021 22:53:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921db7ddca2b72930c0ba65cfcf991843ce2fdee70e5ed022876b6f5bebbe5`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c499f2e405c30092431c8a9e2734154a24af4ed421ff0c7d97b16d1b02f39`  
		Last Modified: Tue, 11 May 2021 00:40:40 GMT  
		Size: 135.7 MB (135656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1d700e09af9f173c1ca948355e0d1a01b5c6139b36889ca0621055669821f9`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99d8d95772dfd5147e631e7e072172ebe7c33d5d8916e8f372607a7c866572`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:8027a70fbe7e47adb3b0970eacbbc1dd78cf06203cf320da5cdbc5cf71d3e01d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037334566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35400f2fef53c6fde1a596644884d280e42c2043b303fb8a64bf09ddebe3d0b5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:33:49 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:33:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:33:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:39:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:39:49 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:39:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa26c3b7dd5be40e6af6e110598ff8ade5597433a780e713fe02d41a01ff4ab`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcc96fa02f1eff07ba750778c31dbc2a2b2eb1205d0862a2ebe6b93c8f2785b`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264615459bc5dd410e8fdba7e066381e9fd687efbafbcbdc04d6a3c8f19ccb5`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93394405d931bc35ec98aec50a2d8664f5c0580f16dbae47c70dabbebf81356d`  
		Last Modified: Wed, 12 May 2021 00:59:03 GMT  
		Size: 241.5 MB (241547428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4854c02134142d249afb7fb7045fd09f266e95fce580e919b709b8dac5572bc`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea254f563aa38c2c7a29f573537255e55d3b9e8ab8c43bd857e1e8ea156bb9c4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0592557aaf1bfb0d38c61451aa21ccc7d3b5e447d85f6e38b920c27ebc0eb7b4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:3dbb3b4b8f33c8a61fa72cf1d05398d6cc09c72aa2a1f664b639d8231b0e83ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:ebb6b8403c1f47069b099f1ba75778d41e15a5d8eed3db6f435733333e403a2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175677269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07630e791de3ceb87d39543799438e118753246d19dcfd6529bd4d27ff1b83bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:58 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 00:41:59 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:11:00 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:11:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:11:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:11:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:11:48 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:11:49 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:11:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:11:49 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:11:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2ff17242ce7e307fbd191a597f210061566606443ff6632ca685d394cb9acf`  
		Last Modified: Sat, 24 Apr 2021 00:44:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11b2ce05942f19ca819aa8c130575b0850153384fba7f489fd1a62ec0d94e7`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91532386f4ec7af743bc43ddbab8410d9d2fee68ce63bca3aa397c04e29b9091`  
		Last Modified: Tue, 11 May 2021 00:12:51 GMT  
		Size: 140.2 MB (140162019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705ef0ab262e766f32008195b4e3719f5444b83e3218dbab09f5cfa7098322ea`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6238126b609f01bb47ddd8598f331bb5cb7653f2d9798eb2f14d48061d8e279`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 4.5 KB (4477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8f2c9016beb50c2972e54c732d8dc24fb332360104b9e71767af9c4e71c1348e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168070890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3a757873434f9961cb2b732f35c712866d65e5fdf009c9b8572d46c0657e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 01:53:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:53:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:08 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 01:41:03 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 01:41:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 01:41:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 01:41:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 01:41:41 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 01:41:42 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 01:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:41:44 GMT
EXPOSE 27017
# Tue, 11 May 2021 01:41:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b8f707197ef2788f2ed0cf82b088b9262efb9b7a374da64bb70daccca6525`  
		Last Modified: Sat, 24 Apr 2021 01:56:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d9f84ef7c607013458b7c4f0045d42081a3cd4e32e09a99c45af7af1742eb`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a71fa0bced6eaef2a94dfda7f28a3c97b1f52e0def1e877932edf84e97df5`  
		Last Modified: Tue, 11 May 2021 01:42:41 GMT  
		Size: 136.3 MB (136341433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88698b947abf4aa832fdbc0c629195e7b8ad1790baad6dfa6ad42b0201e5b81e`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7dfc922696b1eae0c53f3c4559bdfca5ae0dd740a6c3e5166c0839e4ce49ad`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:c8e981f281462baf0c84890eab82c4fad6c825d221664b463ccd43485f6380cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169474559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8b1f024425214a141ef62568a875dc3f443453094dbe43757c3a42d5ada69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:51:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Apr 2021 22:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:51:56 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 22:51:57 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Apr 2021 22:52:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 22:52:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 22:52:19 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 23 Apr 2021 22:52:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:24 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:38:53 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:38:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:39:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:39:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:39:55 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:39:55 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:39:56 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:39:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bc20f34c3c0e6defa11123a46488ad9866f1cbed77d74904f7b057f014902`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934bd72760b936ef87cda05b4fd31a1266859e77f6960e8b6a17eb4df55b82b2`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 2.7 MB (2708330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778576254d798d87ee503dd46947744945440e160227cf20f86506eb7f0c752`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 5.7 MB (5747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b7218def3876e2bd7ede8db669dd67c94e3f67db5c8b385e7d0b189c70f19`  
		Last Modified: Fri, 23 Apr 2021 22:53:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218c55b05ae6da8d768db66caf009228dd32c56943df536e02932cd24a359f1e`  
		Last Modified: Fri, 23 Apr 2021 22:53:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921db7ddca2b72930c0ba65cfcf991843ce2fdee70e5ed022876b6f5bebbe5`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c499f2e405c30092431c8a9e2734154a24af4ed421ff0c7d97b16d1b02f39`  
		Last Modified: Tue, 11 May 2021 00:40:40 GMT  
		Size: 135.7 MB (135656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1d700e09af9f173c1ca948355e0d1a01b5c6139b36889ca0621055669821f9`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99d8d95772dfd5147e631e7e072172ebe7c33d5d8916e8f372607a7c866572`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:eb0c7d46164fd225423e2c0fc64e96f52c38b738f8fd9ccba13e56c4eb119275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `mongo:4-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull mongo@sha256:e2dc6e2ce10059a0d52f2e7ef003b495ed57e72c0b0e00bac2148b20dec63355
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706212737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ddc9cab99b833b8495cc7ee447d7c65463a6c877af4d80d4aa833b6d64b99a5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 10 May 2021 23:15:58 GMT
ENV MONGO_VERSION=4.4.6
# Mon, 10 May 2021 23:15:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Mon, 10 May 2021 23:16:01 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Mon, 10 May 2021 23:18:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 10 May 2021 23:18:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 10 May 2021 23:18:25 GMT
EXPOSE 27017
# Mon, 10 May 2021 23:18:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1af6a38cdaf02b9763a51588fe3ec107b6324e3c240b81be1c53374619c675`  
		Last Modified: Mon, 10 May 2021 23:24:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4550f7fa25bb90c099b1eac08fa398f54f44d40adeb082ad7c38a62223c6a411`  
		Last Modified: Mon, 10 May 2021 23:24:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdfb1c878583e1857a026502bc1d5644702990001c8ed20f4b1b647706c59b`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417a1588a5fc27f1d60b2a2ea14002824a5de37b9d3ad7ccbb2484e44c3a9dcf`  
		Last Modified: Mon, 10 May 2021 23:24:48 GMT  
		Size: 236.4 MB (236448794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed7b32008983c9797db237aa9a90c851d502b47467b518ec9060f17065ca44`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b56283a6d31ef57873809be37e8516d0606ab794493b8237b90eb5b91be6b2`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb68b8b769ff2ae29874c729c09a2db8d3e7e0727b7b486792074d26ff7d802`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull mongo@sha256:2eac7d1f71ed080a26b742240fe92543fe2e940bb5a48fdd59ac3fecc0e9e73c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6036382733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03eb8c7454248dc61a5ae434a904103696979b3e44430a44cedeb70ec3b92a7a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 10 May 2021 23:18:41 GMT
ENV MONGO_VERSION=4.4.6
# Mon, 10 May 2021 23:18:43 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Mon, 10 May 2021 23:18:44 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Mon, 10 May 2021 23:22:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 10 May 2021 23:22:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 10 May 2021 23:22:16 GMT
EXPOSE 27017
# Mon, 10 May 2021 23:22:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b78e3aa88d4e50d3d51ac081c91eeef9933d4a7a75f4845821519ed2bd1a3`  
		Last Modified: Mon, 10 May 2021 23:25:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f41596dd2dda6342571328e8de671fc73c58da781f443547f9bd94b2e602a1a`  
		Last Modified: Mon, 10 May 2021 23:25:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0fd0da468dbf2b3fb5817a9dfe9badc42a5ae933fe238ba533b51dcd548b8`  
		Last Modified: Mon, 10 May 2021 23:25:06 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228c37f48edb438de1305cde961522a16d6041442f1b377b315370fad7c041c`  
		Last Modified: Mon, 10 May 2021 23:26:04 GMT  
		Size: 241.5 MB (241488971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94206c6a1738fc370c80eb4e0259a1a74df12b0c8fa4fd45227cbd18d38bbf1`  
		Last Modified: Mon, 10 May 2021 23:25:05 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4cfcf8250b04c427f36ba05bef1ef1e42cb65e92b9f3cc2fd3f3c4fc976c65`  
		Last Modified: Mon, 10 May 2021 23:25:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0f9cb3fef403e1662a10830f0d076d9cdd0d374fd01875379380b862a41009`  
		Last Modified: Mon, 10 May 2021 23:25:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:8917c43037c70887cbb4140acc128cea9c1c2fd7fcb70257d20145baedbd6fab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:c1c7f59a7f29591106d067877ad4e568d260572adcd9803d1fef162ca4ec9a22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:8027a70fbe7e47adb3b0970eacbbc1dd78cf06203cf320da5cdbc5cf71d3e01d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037334566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35400f2fef53c6fde1a596644884d280e42c2043b303fb8a64bf09ddebe3d0b5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:33:49 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:33:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:33:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:39:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:39:49 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:39:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa26c3b7dd5be40e6af6e110598ff8ade5597433a780e713fe02d41a01ff4ab`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcc96fa02f1eff07ba750778c31dbc2a2b2eb1205d0862a2ebe6b93c8f2785b`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264615459bc5dd410e8fdba7e066381e9fd687efbafbcbdc04d6a3c8f19ccb5`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93394405d931bc35ec98aec50a2d8664f5c0580f16dbae47c70dabbebf81356d`  
		Last Modified: Wed, 12 May 2021 00:59:03 GMT  
		Size: 241.5 MB (241547428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4854c02134142d249afb7fb7045fd09f266e95fce580e919b709b8dac5572bc`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea254f563aa38c2c7a29f573537255e55d3b9e8ab8c43bd857e1e8ea156bb9c4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0592557aaf1bfb0d38c61451aa21ccc7d3b5e447d85f6e38b920c27ebc0eb7b4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:4bdfa331c99ed16c61a9b583142118c1f67ec33a53f8f95c7f8777f4dc15d259
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:eb94bcf4aaf836e31d0fec4ffaad36b2388249af403fccfa1d31bef96429eeda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156442486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8a52aa11b168765286914eff185a785ebf7e8df6a36c3a78fb433001252513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:42 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 24 Apr 2021 00:40:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:43 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:43 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:44 GMT
ENV MONGO_MAJOR=4.0
# Sat, 24 Apr 2021 00:40:44 GMT
ENV MONGO_VERSION=4.0.24
# Sat, 24 Apr 2021 00:40:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:41:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:41:02 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:19 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:19 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e555232f3af9e56da543d5d234e68cddea1bb874a13edeed0e57910d3cf11b6`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d352d41835817fffacf5d96d0b6d1afdee3ee892bc9ad273caff8f70e41279`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0577d10f34f2ffee96c318d2b0acb294bbf1395e9646555793763812e3e9ec`  
		Last Modified: Sat, 24 Apr 2021 00:43:36 GMT  
		Size: 106.0 MB (105966500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf8f29a4010ae4bdb46dd252d21b5f34515e47c7e68c6f31ba68cda1488458a`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96818deeb506a37f5319555cdecdf130c29d1669fda4b8cebaae3c734dc691e`  
		Last Modified: Thu, 06 May 2021 23:36:08 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ae350f0f6827ffbb93d4390635872968a986248c15014e47406b6a4a09e0d78d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145042509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f56049410a547b49a70bc41914e1ed27e01299214b2e3df8c31603950676f2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:49:23 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 24 Apr 2021 01:49:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:49:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:49:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:49:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:49:31 GMT
ENV MONGO_MAJOR=4.0
# Sat, 24 Apr 2021 01:49:36 GMT
ENV MONGO_VERSION=4.0.24
# Sat, 24 Apr 2021 01:49:46 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:50:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:50:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:50:39 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:46 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:49 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4225029f40c12c7871704ef31a1d58bfb1740338cc851bd7ed9b62a57331129`  
		Last Modified: Sat, 24 Apr 2021 01:55:04 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef359208b6dd08bd9fc4031c7d113add560e3ee71fe5c1285d6e26c5cb8338dd`  
		Last Modified: Sat, 24 Apr 2021 01:55:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c085d22d7b01be33b64ec53036ecc7b5add3584a5cfc603ca653a6169e0f7f01`  
		Last Modified: Sat, 24 Apr 2021 01:55:26 GMT  
		Size: 100.3 MB (100339495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200c8a635a1ea8a0686be9debbfb64216fa3452d894bcf3a5eb1ead703707f55`  
		Last Modified: Sat, 24 Apr 2021 01:55:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2af057c25d56017339359d97f3a9344f516e8ad79e3256be8d6c2c3357266a`  
		Last Modified: Fri, 07 May 2021 01:19:47 GMT  
		Size: 4.5 KB (4473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:3510ec00a6785f3b7b25ab4df2a0b84ebd93c85177d57abb292f7ad63d275585
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706087641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f0bdeab870a7bb34e462bab1afddb842dafcf9fe0128a8f64bb273114969d3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:03:19 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:03:20 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:03:22 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:08:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:08:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:08:40 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:08:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702d6bf6ce121bbbcfa931a1ced8d066b11fe81e341f54c8d2f7feded385c196`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b201f9f9f7c0285ba5f407d32e6945eba3c54f5beb833f4420504aa946b37ab8`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57100ec2ccb18ca6062b55ea8c547cd4317f6beac14d89ddfa3316b274593b80`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524beab8f07400be20b1e7c973847429b185995ba2ceed101a32ea9f7fb89444`  
		Last Modified: Wed, 12 May 2021 00:49:25 GMT  
		Size: 231.6 MB (231588459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aae7ebb19554d5bd6dd318739e10b2448f280998e807add136156eb7d6f7c0`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93444b9c89f8b973bd4a3ab54fab180fcd18e62accef44f052b0899e99129f11`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b32d5b0f807ae8f3d7ed5bee285c8e9d89ec6b584b81fd70730633a4e3f150e`  
		Last Modified: Wed, 12 May 2021 00:48:06 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:65e5d046b0e5d386e4dcdf77b8c10835fd6b4041ea054cc67d1edf770da08db0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032426531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfa6e8351e6e4a9afc61f0053acda064a7b25c10bafc76d4d61efca1aabaf65`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:09:08 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:09:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:09:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:17:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:17:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:17:23 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:17:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc8ee3ad2c865ead346641f2c46a1de9fc4ff7b296474dfa9f4fa437dcc75d`  
		Last Modified: Wed, 12 May 2021 00:49:44 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e22165f2030c3e954c477e1e3ebe8efd0953956e39283685765f5f80d699b`  
		Last Modified: Wed, 12 May 2021 00:49:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60cab09b435ef4269fc96a5821263d682ed138fc506c1e429998d8677e42965`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2fddb5f64fca72ef3d539bd2aa2030a87fcf63091475d2f2ae5a53cefec02f`  
		Last Modified: Wed, 12 May 2021 00:50:35 GMT  
		Size: 236.6 MB (236639148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9273acde3f5cd073066fe43c216f8959fe67cd0d1834fba08dab8ffae2e61efe`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d615f474f823d1be785307a62e233039281ce1d919a71c827beca88c2007d9`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4e395df061109a0c3ce6f3bf338e27eeeb82a0e1a98a22cf9fd180844d6c6`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:fd4babec8bf3d29bb4a0c9149af2d80f88bfb75fbe695fb72d98b8de6de77d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:3510ec00a6785f3b7b25ab4df2a0b84ebd93c85177d57abb292f7ad63d275585
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706087641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f0bdeab870a7bb34e462bab1afddb842dafcf9fe0128a8f64bb273114969d3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:03:19 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:03:20 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:03:22 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:08:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:08:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:08:40 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:08:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702d6bf6ce121bbbcfa931a1ced8d066b11fe81e341f54c8d2f7feded385c196`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b201f9f9f7c0285ba5f407d32e6945eba3c54f5beb833f4420504aa946b37ab8`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57100ec2ccb18ca6062b55ea8c547cd4317f6beac14d89ddfa3316b274593b80`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524beab8f07400be20b1e7c973847429b185995ba2ceed101a32ea9f7fb89444`  
		Last Modified: Wed, 12 May 2021 00:49:25 GMT  
		Size: 231.6 MB (231588459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aae7ebb19554d5bd6dd318739e10b2448f280998e807add136156eb7d6f7c0`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93444b9c89f8b973bd4a3ab54fab180fcd18e62accef44f052b0899e99129f11`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b32d5b0f807ae8f3d7ed5bee285c8e9d89ec6b584b81fd70730633a4e3f150e`  
		Last Modified: Wed, 12 May 2021 00:48:06 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:65e5d046b0e5d386e4dcdf77b8c10835fd6b4041ea054cc67d1edf770da08db0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032426531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfa6e8351e6e4a9afc61f0053acda064a7b25c10bafc76d4d61efca1aabaf65`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:09:08 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:09:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:09:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:17:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:17:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:17:23 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:17:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc8ee3ad2c865ead346641f2c46a1de9fc4ff7b296474dfa9f4fa437dcc75d`  
		Last Modified: Wed, 12 May 2021 00:49:44 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e22165f2030c3e954c477e1e3ebe8efd0953956e39283685765f5f80d699b`  
		Last Modified: Wed, 12 May 2021 00:49:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60cab09b435ef4269fc96a5821263d682ed138fc506c1e429998d8677e42965`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2fddb5f64fca72ef3d539bd2aa2030a87fcf63091475d2f2ae5a53cefec02f`  
		Last Modified: Wed, 12 May 2021 00:50:35 GMT  
		Size: 236.6 MB (236639148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9273acde3f5cd073066fe43c216f8959fe67cd0d1834fba08dab8ffae2e61efe`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d615f474f823d1be785307a62e233039281ce1d919a71c827beca88c2007d9`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4e395df061109a0c3ce6f3bf338e27eeeb82a0e1a98a22cf9fd180844d6c6`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:05041092969f34f102158d86cba4956e445d1454648ae8ea3b777d122cd628d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:3510ec00a6785f3b7b25ab4df2a0b84ebd93c85177d57abb292f7ad63d275585
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706087641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f0bdeab870a7bb34e462bab1afddb842dafcf9fe0128a8f64bb273114969d3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:03:19 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:03:20 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:03:22 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:08:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:08:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:08:40 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:08:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702d6bf6ce121bbbcfa931a1ced8d066b11fe81e341f54c8d2f7feded385c196`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b201f9f9f7c0285ba5f407d32e6945eba3c54f5beb833f4420504aa946b37ab8`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57100ec2ccb18ca6062b55ea8c547cd4317f6beac14d89ddfa3316b274593b80`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524beab8f07400be20b1e7c973847429b185995ba2ceed101a32ea9f7fb89444`  
		Last Modified: Wed, 12 May 2021 00:49:25 GMT  
		Size: 231.6 MB (231588459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aae7ebb19554d5bd6dd318739e10b2448f280998e807add136156eb7d6f7c0`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93444b9c89f8b973bd4a3ab54fab180fcd18e62accef44f052b0899e99129f11`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b32d5b0f807ae8f3d7ed5bee285c8e9d89ec6b584b81fd70730633a4e3f150e`  
		Last Modified: Wed, 12 May 2021 00:48:06 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:4cdcd5e3bc3388180bef96dced0b822efa6013437b168c174af84ebe5c5f9a78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:65e5d046b0e5d386e4dcdf77b8c10835fd6b4041ea054cc67d1edf770da08db0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032426531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfa6e8351e6e4a9afc61f0053acda064a7b25c10bafc76d4d61efca1aabaf65`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:09:08 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:09:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:09:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:17:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:17:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:17:23 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:17:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc8ee3ad2c865ead346641f2c46a1de9fc4ff7b296474dfa9f4fa437dcc75d`  
		Last Modified: Wed, 12 May 2021 00:49:44 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e22165f2030c3e954c477e1e3ebe8efd0953956e39283685765f5f80d699b`  
		Last Modified: Wed, 12 May 2021 00:49:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60cab09b435ef4269fc96a5821263d682ed138fc506c1e429998d8677e42965`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2fddb5f64fca72ef3d539bd2aa2030a87fcf63091475d2f2ae5a53cefec02f`  
		Last Modified: Wed, 12 May 2021 00:50:35 GMT  
		Size: 236.6 MB (236639148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9273acde3f5cd073066fe43c216f8959fe67cd0d1834fba08dab8ffae2e61efe`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d615f474f823d1be785307a62e233039281ce1d919a71c827beca88c2007d9`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4e395df061109a0c3ce6f3bf338e27eeeb82a0e1a98a22cf9fd180844d6c6`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:fa2582b00bac68fbb66c07fce5ce3555fd217a3f28e7c320e4972f7a24c185f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:eb94bcf4aaf836e31d0fec4ffaad36b2388249af403fccfa1d31bef96429eeda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156442486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8a52aa11b168765286914eff185a785ebf7e8df6a36c3a78fb433001252513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:42 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 24 Apr 2021 00:40:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:43 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:43 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:44 GMT
ENV MONGO_MAJOR=4.0
# Sat, 24 Apr 2021 00:40:44 GMT
ENV MONGO_VERSION=4.0.24
# Sat, 24 Apr 2021 00:40:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:41:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:41:02 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:19 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:19 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e555232f3af9e56da543d5d234e68cddea1bb874a13edeed0e57910d3cf11b6`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d352d41835817fffacf5d96d0b6d1afdee3ee892bc9ad273caff8f70e41279`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0577d10f34f2ffee96c318d2b0acb294bbf1395e9646555793763812e3e9ec`  
		Last Modified: Sat, 24 Apr 2021 00:43:36 GMT  
		Size: 106.0 MB (105966500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf8f29a4010ae4bdb46dd252d21b5f34515e47c7e68c6f31ba68cda1488458a`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96818deeb506a37f5319555cdecdf130c29d1669fda4b8cebaae3c734dc691e`  
		Last Modified: Thu, 06 May 2021 23:36:08 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ae350f0f6827ffbb93d4390635872968a986248c15014e47406b6a4a09e0d78d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145042509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f56049410a547b49a70bc41914e1ed27e01299214b2e3df8c31603950676f2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:49:23 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 24 Apr 2021 01:49:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:49:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:49:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:49:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:49:31 GMT
ENV MONGO_MAJOR=4.0
# Sat, 24 Apr 2021 01:49:36 GMT
ENV MONGO_VERSION=4.0.24
# Sat, 24 Apr 2021 01:49:46 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:50:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:50:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:50:39 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:46 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:49 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4225029f40c12c7871704ef31a1d58bfb1740338cc851bd7ed9b62a57331129`  
		Last Modified: Sat, 24 Apr 2021 01:55:04 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef359208b6dd08bd9fc4031c7d113add560e3ee71fe5c1285d6e26c5cb8338dd`  
		Last Modified: Sat, 24 Apr 2021 01:55:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c085d22d7b01be33b64ec53036ecc7b5add3584a5cfc603ca653a6169e0f7f01`  
		Last Modified: Sat, 24 Apr 2021 01:55:26 GMT  
		Size: 100.3 MB (100339495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200c8a635a1ea8a0686be9debbfb64216fa3452d894bcf3a5eb1ead703707f55`  
		Last Modified: Sat, 24 Apr 2021 01:55:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2af057c25d56017339359d97f3a9344f516e8ad79e3256be8d6c2c3357266a`  
		Last Modified: Fri, 07 May 2021 01:19:47 GMT  
		Size: 4.5 KB (4473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.24`

```console
$ docker pull mongo@sha256:4bdfa331c99ed16c61a9b583142118c1f67ec33a53f8f95c7f8777f4dc15d259
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.0.24` - linux; amd64

```console
$ docker pull mongo@sha256:eb94bcf4aaf836e31d0fec4ffaad36b2388249af403fccfa1d31bef96429eeda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156442486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8a52aa11b168765286914eff185a785ebf7e8df6a36c3a78fb433001252513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:42 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 24 Apr 2021 00:40:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:43 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:43 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:44 GMT
ENV MONGO_MAJOR=4.0
# Sat, 24 Apr 2021 00:40:44 GMT
ENV MONGO_VERSION=4.0.24
# Sat, 24 Apr 2021 00:40:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:41:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:41:02 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:19 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:19 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e555232f3af9e56da543d5d234e68cddea1bb874a13edeed0e57910d3cf11b6`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d352d41835817fffacf5d96d0b6d1afdee3ee892bc9ad273caff8f70e41279`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0577d10f34f2ffee96c318d2b0acb294bbf1395e9646555793763812e3e9ec`  
		Last Modified: Sat, 24 Apr 2021 00:43:36 GMT  
		Size: 106.0 MB (105966500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf8f29a4010ae4bdb46dd252d21b5f34515e47c7e68c6f31ba68cda1488458a`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96818deeb506a37f5319555cdecdf130c29d1669fda4b8cebaae3c734dc691e`  
		Last Modified: Thu, 06 May 2021 23:36:08 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.24` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ae350f0f6827ffbb93d4390635872968a986248c15014e47406b6a4a09e0d78d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145042509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f56049410a547b49a70bc41914e1ed27e01299214b2e3df8c31603950676f2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:49:23 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 24 Apr 2021 01:49:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:49:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:49:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:49:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:49:31 GMT
ENV MONGO_MAJOR=4.0
# Sat, 24 Apr 2021 01:49:36 GMT
ENV MONGO_VERSION=4.0.24
# Sat, 24 Apr 2021 01:49:46 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:50:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:50:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:50:39 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:46 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:49 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4225029f40c12c7871704ef31a1d58bfb1740338cc851bd7ed9b62a57331129`  
		Last Modified: Sat, 24 Apr 2021 01:55:04 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef359208b6dd08bd9fc4031c7d113add560e3ee71fe5c1285d6e26c5cb8338dd`  
		Last Modified: Sat, 24 Apr 2021 01:55:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c085d22d7b01be33b64ec53036ecc7b5add3584a5cfc603ca653a6169e0f7f01`  
		Last Modified: Sat, 24 Apr 2021 01:55:26 GMT  
		Size: 100.3 MB (100339495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200c8a635a1ea8a0686be9debbfb64216fa3452d894bcf3a5eb1ead703707f55`  
		Last Modified: Sat, 24 Apr 2021 01:55:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2af057c25d56017339359d97f3a9344f516e8ad79e3256be8d6c2c3357266a`  
		Last Modified: Fri, 07 May 2021 01:19:47 GMT  
		Size: 4.5 KB (4473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.24` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:3510ec00a6785f3b7b25ab4df2a0b84ebd93c85177d57abb292f7ad63d275585
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706087641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f0bdeab870a7bb34e462bab1afddb842dafcf9fe0128a8f64bb273114969d3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:03:19 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:03:20 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:03:22 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:08:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:08:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:08:40 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:08:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702d6bf6ce121bbbcfa931a1ced8d066b11fe81e341f54c8d2f7feded385c196`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b201f9f9f7c0285ba5f407d32e6945eba3c54f5beb833f4420504aa946b37ab8`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57100ec2ccb18ca6062b55ea8c547cd4317f6beac14d89ddfa3316b274593b80`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524beab8f07400be20b1e7c973847429b185995ba2ceed101a32ea9f7fb89444`  
		Last Modified: Wed, 12 May 2021 00:49:25 GMT  
		Size: 231.6 MB (231588459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aae7ebb19554d5bd6dd318739e10b2448f280998e807add136156eb7d6f7c0`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93444b9c89f8b973bd4a3ab54fab180fcd18e62accef44f052b0899e99129f11`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b32d5b0f807ae8f3d7ed5bee285c8e9d89ec6b584b81fd70730633a4e3f150e`  
		Last Modified: Wed, 12 May 2021 00:48:06 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.24` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:65e5d046b0e5d386e4dcdf77b8c10835fd6b4041ea054cc67d1edf770da08db0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032426531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfa6e8351e6e4a9afc61f0053acda064a7b25c10bafc76d4d61efca1aabaf65`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:09:08 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:09:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:09:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:17:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:17:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:17:23 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:17:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc8ee3ad2c865ead346641f2c46a1de9fc4ff7b296474dfa9f4fa437dcc75d`  
		Last Modified: Wed, 12 May 2021 00:49:44 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e22165f2030c3e954c477e1e3ebe8efd0953956e39283685765f5f80d699b`  
		Last Modified: Wed, 12 May 2021 00:49:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60cab09b435ef4269fc96a5821263d682ed138fc506c1e429998d8677e42965`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2fddb5f64fca72ef3d539bd2aa2030a87fcf63091475d2f2ae5a53cefec02f`  
		Last Modified: Wed, 12 May 2021 00:50:35 GMT  
		Size: 236.6 MB (236639148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9273acde3f5cd073066fe43c216f8959fe67cd0d1834fba08dab8ffae2e61efe`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d615f474f823d1be785307a62e233039281ce1d919a71c827beca88c2007d9`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4e395df061109a0c3ce6f3bf338e27eeeb82a0e1a98a22cf9fd180844d6c6`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.24-windowsservercore`

```console
$ docker pull mongo@sha256:fd4babec8bf3d29bb4a0c9149af2d80f88bfb75fbe695fb72d98b8de6de77d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.0.24-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:3510ec00a6785f3b7b25ab4df2a0b84ebd93c85177d57abb292f7ad63d275585
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706087641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f0bdeab870a7bb34e462bab1afddb842dafcf9fe0128a8f64bb273114969d3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:03:19 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:03:20 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:03:22 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:08:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:08:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:08:40 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:08:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702d6bf6ce121bbbcfa931a1ced8d066b11fe81e341f54c8d2f7feded385c196`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b201f9f9f7c0285ba5f407d32e6945eba3c54f5beb833f4420504aa946b37ab8`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57100ec2ccb18ca6062b55ea8c547cd4317f6beac14d89ddfa3316b274593b80`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524beab8f07400be20b1e7c973847429b185995ba2ceed101a32ea9f7fb89444`  
		Last Modified: Wed, 12 May 2021 00:49:25 GMT  
		Size: 231.6 MB (231588459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aae7ebb19554d5bd6dd318739e10b2448f280998e807add136156eb7d6f7c0`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93444b9c89f8b973bd4a3ab54fab180fcd18e62accef44f052b0899e99129f11`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b32d5b0f807ae8f3d7ed5bee285c8e9d89ec6b584b81fd70730633a4e3f150e`  
		Last Modified: Wed, 12 May 2021 00:48:06 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.24-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:65e5d046b0e5d386e4dcdf77b8c10835fd6b4041ea054cc67d1edf770da08db0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032426531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfa6e8351e6e4a9afc61f0053acda064a7b25c10bafc76d4d61efca1aabaf65`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:09:08 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:09:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:09:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:17:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:17:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:17:23 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:17:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc8ee3ad2c865ead346641f2c46a1de9fc4ff7b296474dfa9f4fa437dcc75d`  
		Last Modified: Wed, 12 May 2021 00:49:44 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e22165f2030c3e954c477e1e3ebe8efd0953956e39283685765f5f80d699b`  
		Last Modified: Wed, 12 May 2021 00:49:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60cab09b435ef4269fc96a5821263d682ed138fc506c1e429998d8677e42965`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2fddb5f64fca72ef3d539bd2aa2030a87fcf63091475d2f2ae5a53cefec02f`  
		Last Modified: Wed, 12 May 2021 00:50:35 GMT  
		Size: 236.6 MB (236639148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9273acde3f5cd073066fe43c216f8959fe67cd0d1834fba08dab8ffae2e61efe`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d615f474f823d1be785307a62e233039281ce1d919a71c827beca88c2007d9`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4e395df061109a0c3ce6f3bf338e27eeeb82a0e1a98a22cf9fd180844d6c6`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.24-windowsservercore-1809`

```console
$ docker pull mongo@sha256:05041092969f34f102158d86cba4956e445d1454648ae8ea3b777d122cd628d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:4.0.24-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:3510ec00a6785f3b7b25ab4df2a0b84ebd93c85177d57abb292f7ad63d275585
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706087641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f0bdeab870a7bb34e462bab1afddb842dafcf9fe0128a8f64bb273114969d3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:03:19 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:03:20 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:03:22 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:08:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:08:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:08:40 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:08:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702d6bf6ce121bbbcfa931a1ced8d066b11fe81e341f54c8d2f7feded385c196`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b201f9f9f7c0285ba5f407d32e6945eba3c54f5beb833f4420504aa946b37ab8`  
		Last Modified: Wed, 12 May 2021 00:48:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57100ec2ccb18ca6062b55ea8c547cd4317f6beac14d89ddfa3316b274593b80`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524beab8f07400be20b1e7c973847429b185995ba2ceed101a32ea9f7fb89444`  
		Last Modified: Wed, 12 May 2021 00:49:25 GMT  
		Size: 231.6 MB (231588459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aae7ebb19554d5bd6dd318739e10b2448f280998e807add136156eb7d6f7c0`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93444b9c89f8b973bd4a3ab54fab180fcd18e62accef44f052b0899e99129f11`  
		Last Modified: Wed, 12 May 2021 00:48:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b32d5b0f807ae8f3d7ed5bee285c8e9d89ec6b584b81fd70730633a4e3f150e`  
		Last Modified: Wed, 12 May 2021 00:48:06 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.24-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:4cdcd5e3bc3388180bef96dced0b822efa6013437b168c174af84ebe5c5f9a78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.0.24-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:65e5d046b0e5d386e4dcdf77b8c10835fd6b4041ea054cc67d1edf770da08db0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032426531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfa6e8351e6e4a9afc61f0053acda064a7b25c10bafc76d4d61efca1aabaf65`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:09:08 GMT
ENV MONGO_VERSION=4.0.24
# Wed, 12 May 2021 00:09:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.24-signed.msi
# Wed, 12 May 2021 00:09:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e17a25bc51b6bdcf6da0fe6b0ba22075b43566119c656b454542735133cd9f1e
# Wed, 12 May 2021 00:17:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:17:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:17:23 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:17:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc8ee3ad2c865ead346641f2c46a1de9fc4ff7b296474dfa9f4fa437dcc75d`  
		Last Modified: Wed, 12 May 2021 00:49:44 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e22165f2030c3e954c477e1e3ebe8efd0953956e39283685765f5f80d699b`  
		Last Modified: Wed, 12 May 2021 00:49:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60cab09b435ef4269fc96a5821263d682ed138fc506c1e429998d8677e42965`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2fddb5f64fca72ef3d539bd2aa2030a87fcf63091475d2f2ae5a53cefec02f`  
		Last Modified: Wed, 12 May 2021 00:50:35 GMT  
		Size: 236.6 MB (236639148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9273acde3f5cd073066fe43c216f8959fe67cd0d1834fba08dab8ffae2e61efe`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d615f474f823d1be785307a62e233039281ce1d919a71c827beca88c2007d9`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4e395df061109a0c3ce6f3bf338e27eeeb82a0e1a98a22cf9fd180844d6c6`  
		Last Modified: Wed, 12 May 2021 00:49:41 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.24-xenial`

```console
$ docker pull mongo@sha256:fa2582b00bac68fbb66c07fce5ce3555fd217a3f28e7c320e4972f7a24c185f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.24-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:eb94bcf4aaf836e31d0fec4ffaad36b2388249af403fccfa1d31bef96429eeda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156442486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8a52aa11b168765286914eff185a785ebf7e8df6a36c3a78fb433001252513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:22:16 GMT
ADD file:34f9c325bb2e6ad9f9a062ce9a0237fab0c04aea83f31b8548ea0ae532255be0 in / 
# Fri, 23 Apr 2021 22:22:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:22:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:22:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:22:19 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:39:31 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:39:43 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:39:43 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:40:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:40:42 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 24 Apr 2021 00:40:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:40:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:40:43 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:43 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:40:44 GMT
ENV MONGO_MAJOR=4.0
# Sat, 24 Apr 2021 00:40:44 GMT
ENV MONGO_VERSION=4.0.24
# Sat, 24 Apr 2021 00:40:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 00:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 00:41:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 00:41:02 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:19 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:19 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92473f7ef45574f608989888a6cfc8187d3a1425e3a63f974434acab03fed068`  
		Last Modified: Sat, 17 Apr 2021 15:20:07 GMT  
		Size: 46.3 MB (46254451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb52bde70123ac7f3a1b88fee95e74f4bdcdbd81917a91a35b56a52ec7671947`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64788f86be3fd71809b5de602deff9445f3de18d2f44a49d0a053dfc9a2008ae`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f6d5f2e001ababe3ddac4731d9c33121e1148ef32a87a83a5b470cb401abef`  
		Last Modified: Fri, 23 Apr 2021 22:24:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e566566088ce28562fe7f49c1b8aff253759e0b5eb68127893c93a45d3788`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518a872ab12ebcda66545c2d28ffd61ff22e8fbae0a597f5e635420a49d1e17`  
		Last Modified: Sat, 24 Apr 2021 00:42:53 GMT  
		Size: 2.9 MB (2906253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bdae151f641abb1f44895e54086449e071860cc91845db474fa031e7ed8dbc`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 1.3 MB (1305291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c58da5f5635ea471bc09287e13e1b3a0df3c02b471be8c0cc08c0975871a69`  
		Last Modified: Sat, 24 Apr 2021 00:42:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e555232f3af9e56da543d5d234e68cddea1bb874a13edeed0e57910d3cf11b6`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d352d41835817fffacf5d96d0b6d1afdee3ee892bc9ad273caff8f70e41279`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0577d10f34f2ffee96c318d2b0acb294bbf1395e9646555793763812e3e9ec`  
		Last Modified: Sat, 24 Apr 2021 00:43:36 GMT  
		Size: 106.0 MB (105966500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf8f29a4010ae4bdb46dd252d21b5f34515e47c7e68c6f31ba68cda1488458a`  
		Last Modified: Sat, 24 Apr 2021 00:43:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96818deeb506a37f5319555cdecdf130c29d1669fda4b8cebaae3c734dc691e`  
		Last Modified: Thu, 06 May 2021 23:36:08 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.24-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ae350f0f6827ffbb93d4390635872968a986248c15014e47406b6a4a09e0d78d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145042509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f56049410a547b49a70bc41914e1ed27e01299214b2e3df8c31603950676f2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:47:17 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:47:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:47:36 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:47:37 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:48:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:49:23 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 24 Apr 2021 01:49:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:49:27 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:49:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:49:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:49:31 GMT
ENV MONGO_MAJOR=4.0
# Sat, 24 Apr 2021 01:49:36 GMT
ENV MONGO_VERSION=4.0.24
# Sat, 24 Apr 2021 01:49:46 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 24 Apr 2021 01:50:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 24 Apr 2021 01:50:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 24 Apr 2021 01:50:39 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:18:46 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:18:49 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:18:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0f5b64b9a877ccee2dbda84065dfa1b6b1e8092aa7412bdd2de314a14427a5`  
		Last Modified: Sat, 24 Apr 2021 01:54:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b5958d6d6adb49f9e258f79a552e004d013ae823ffa19b91a2b2134dccf20`  
		Last Modified: Sat, 24 Apr 2021 01:54:28 GMT  
		Size: 2.4 MB (2434299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0eaefdfeee135c1dcf57f11ad9310b82d75191b23bbe26720bd446ae7416`  
		Last Modified: Sat, 24 Apr 2021 01:54:26 GMT  
		Size: 1.2 MB (1232017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf0613beedf0c9e4cf41bb51dae19841e0d8c637ecb68b62ad1fc6f576b006`  
		Last Modified: Sat, 24 Apr 2021 01:54:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4225029f40c12c7871704ef31a1d58bfb1740338cc851bd7ed9b62a57331129`  
		Last Modified: Sat, 24 Apr 2021 01:55:04 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef359208b6dd08bd9fc4031c7d113add560e3ee71fe5c1285d6e26c5cb8338dd`  
		Last Modified: Sat, 24 Apr 2021 01:55:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c085d22d7b01be33b64ec53036ecc7b5add3584a5cfc603ca653a6169e0f7f01`  
		Last Modified: Sat, 24 Apr 2021 01:55:26 GMT  
		Size: 100.3 MB (100339495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200c8a635a1ea8a0686be9debbfb64216fa3452d894bcf3a5eb1ead703707f55`  
		Last Modified: Sat, 24 Apr 2021 01:55:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2af057c25d56017339359d97f3a9344f516e8ad79e3256be8d6c2c3357266a`  
		Last Modified: Fri, 07 May 2021 01:19:47 GMT  
		Size: 4.5 KB (4473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:5c3059c8191861aaf766ce1ac592ebb42ea71ff13951701049bca93e8d614f96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:641c065374d80202ef8ca35c6685832ff08feab9373728fe10038af85aefc645
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165072113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc77715107a90808446742859973f659a3328a979c9d5f420267ecc27353d7b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:29 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 24 Apr 2021 00:41:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:41:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:41:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:41:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:41:31 GMT
ENV MONGO_MAJOR=4.2
# Thu, 06 May 2021 21:19:37 GMT
ENV MONGO_VERSION=4.2.14
# Thu, 06 May 2021 21:19:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 06 May 2021 21:20:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 06 May 2021 21:20:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 06 May 2021 21:20:22 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:23 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:23 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e22c3240221da2469e6e3cc16eea1d29eb13c4bd9cf2fc47603c8b2aed76bf9`  
		Last Modified: Sat, 24 Apr 2021 00:43:49 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30a5431c1beafcc66aea5e2b40a4563110db168246de911f887088d1bffb074`  
		Last Modified: Thu, 06 May 2021 21:21:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a8fafb4cd8e24a41a87c2a38a0834d2448d6f48d1adacd89063360fa3beeb5`  
		Last Modified: Thu, 06 May 2021 21:21:28 GMT  
		Size: 129.6 MB (129556866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e86f8d8fafd6007157f60c327ca170ea84102643514aae6c543be5a70eb6d8`  
		Last Modified: Thu, 06 May 2021 21:21:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c56df947a8a8f46909dc1b87c276ea136819a33f08b63f0f63ea7e61789e00e`  
		Last Modified: Thu, 06 May 2021 23:36:19 GMT  
		Size: 4.5 KB (4476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:79be37da4cc14b5b16baa1cab614bfa5e9b716994cf37a7b02f877429d924efc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155087094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e99546a4b825ada2a61c060757d85930f463c815086cd80bc6888f838a5aef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:51:43 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 24 Apr 2021 01:51:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:51:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:51:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:51:56 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:51:58 GMT
ENV MONGO_MAJOR=4.2
# Thu, 06 May 2021 19:15:43 GMT
ENV MONGO_VERSION=4.2.14
# Thu, 06 May 2021 19:15:47 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 06 May 2021 19:16:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 06 May 2021 19:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 06 May 2021 19:16:25 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:19:02 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:19:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:19:04 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:19:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e8f8e5e40c62eec6f8ce68e5746d9f4fbaab0274a2f613e2f1d5f7439050e`  
		Last Modified: Sat, 24 Apr 2021 01:55:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9d41cfdf0739861bf0e4c14df5e93bbaa099e91a6cc2b7216f8aebb927cb36`  
		Last Modified: Thu, 06 May 2021 19:17:06 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d29221a58b621dd1174f266c393ca3cc0f41514bd78d636080be446730fe3`  
		Last Modified: Thu, 06 May 2021 19:17:31 GMT  
		Size: 123.4 MB (123357635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47de4b46f14ac681b5b70ec05b23c320169f35b243defe2ac4989706bde1fd`  
		Last Modified: Thu, 06 May 2021 19:17:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9cc492f2ab4768092dd4ee65dda48b96ba0b078d873324033e9f78f143c3f`  
		Last Modified: Fri, 07 May 2021 01:19:53 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:f16d74a62cf3f36dc0ac5167cbe244aeea0f86fdda9436815f3b3f972d6142b8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762028419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3558140470646ef42a86763f4b03a4309b61d072624f02db29c4bb8d8074b603`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:17:45 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:17:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:17:51 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:21:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:21:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:21:56 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:21:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5084dad826c0c649041897fde59f2f8a29657aa36c87dd0ca01f8378e2ac09`  
		Last Modified: Wed, 12 May 2021 00:50:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497aaa432c047dc516f3c3746627b20f533ef1d3f326d30ea81ff17b862cb76`  
		Last Modified: Wed, 12 May 2021 00:50:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a6d0366ca7a4a28b6b3e907dd88321d0b99d180fe40e46823196b1a5660849`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bc979d308d872e587349eb82ed7c3deca66071069c720289c500958a66fd37`  
		Last Modified: Wed, 12 May 2021 00:51:52 GMT  
		Size: 287.5 MB (287529301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2206506a92dd9bb5e31fd2690a0587bf9b991a7fff77a8adf8debed039a06e6c`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5721150e73a1b0b3fda4086694b5ae65dde321f33568ed2ede9181b4e5ec709b`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced697788b22eeb4cc380add1d86cf0e529eff5166667d0bb7ea1e2978344544`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:7afa0ae0c26ab1fc0de929d6db3c346fb460ee5340f37d9d5ef8075009d1ab81
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088400521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92591f36b34947f6d14367125172e6237635b79a73fd82dc0674aed20d50202`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:22:19 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:22:21 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:22:24 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:28:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:28:12 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:28:14 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:28:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64101d9b7b40bb5c07101ee6fe77973e5f71d74067f4fca6c64f66423e12ec`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775b49a444eb1bf0c1179a704f2f8cb229c0e7d4cc6d3cdcd098de593a7c9455`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21c661196aed0c6d9d732de3fcda2f079cc3a018f81c2f23c9437333a9c807`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b3290d98042dcbef7e5d2589d8a45dab1f9ef8902a3f2aff55042694c7950`  
		Last Modified: Wed, 12 May 2021 00:53:12 GMT  
		Size: 292.6 MB (292613155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186bb0a3b7d0556de16f08bb4fff7502c052527541f637637db3d9b4fb39abc`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5399e68624877eb89ac01abbe8edf59e0126b9100e65cb25306e495dc0ca2150`  
		Last Modified: Wed, 12 May 2021 00:52:07 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3112946af906f623bc85ba3e6feb706023451eae47c618b8a861d21fcd34e9`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:d5b168f0e913255d0383fad82222f314cc1f6253add9c8bdbdac11aecabccf7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:641c065374d80202ef8ca35c6685832ff08feab9373728fe10038af85aefc645
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165072113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc77715107a90808446742859973f659a3328a979c9d5f420267ecc27353d7b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:29 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 24 Apr 2021 00:41:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:41:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:41:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:41:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:41:31 GMT
ENV MONGO_MAJOR=4.2
# Thu, 06 May 2021 21:19:37 GMT
ENV MONGO_VERSION=4.2.14
# Thu, 06 May 2021 21:19:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 06 May 2021 21:20:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 06 May 2021 21:20:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 06 May 2021 21:20:22 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:23 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:23 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e22c3240221da2469e6e3cc16eea1d29eb13c4bd9cf2fc47603c8b2aed76bf9`  
		Last Modified: Sat, 24 Apr 2021 00:43:49 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30a5431c1beafcc66aea5e2b40a4563110db168246de911f887088d1bffb074`  
		Last Modified: Thu, 06 May 2021 21:21:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a8fafb4cd8e24a41a87c2a38a0834d2448d6f48d1adacd89063360fa3beeb5`  
		Last Modified: Thu, 06 May 2021 21:21:28 GMT  
		Size: 129.6 MB (129556866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e86f8d8fafd6007157f60c327ca170ea84102643514aae6c543be5a70eb6d8`  
		Last Modified: Thu, 06 May 2021 21:21:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c56df947a8a8f46909dc1b87c276ea136819a33f08b63f0f63ea7e61789e00e`  
		Last Modified: Thu, 06 May 2021 23:36:19 GMT  
		Size: 4.5 KB (4476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:79be37da4cc14b5b16baa1cab614bfa5e9b716994cf37a7b02f877429d924efc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155087094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e99546a4b825ada2a61c060757d85930f463c815086cd80bc6888f838a5aef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:51:43 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 24 Apr 2021 01:51:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:51:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:51:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:51:56 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:51:58 GMT
ENV MONGO_MAJOR=4.2
# Thu, 06 May 2021 19:15:43 GMT
ENV MONGO_VERSION=4.2.14
# Thu, 06 May 2021 19:15:47 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 06 May 2021 19:16:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 06 May 2021 19:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 06 May 2021 19:16:25 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:19:02 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:19:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:19:04 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:19:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e8f8e5e40c62eec6f8ce68e5746d9f4fbaab0274a2f613e2f1d5f7439050e`  
		Last Modified: Sat, 24 Apr 2021 01:55:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9d41cfdf0739861bf0e4c14df5e93bbaa099e91a6cc2b7216f8aebb927cb36`  
		Last Modified: Thu, 06 May 2021 19:17:06 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d29221a58b621dd1174f266c393ca3cc0f41514bd78d636080be446730fe3`  
		Last Modified: Thu, 06 May 2021 19:17:31 GMT  
		Size: 123.4 MB (123357635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47de4b46f14ac681b5b70ec05b23c320169f35b243defe2ac4989706bde1fd`  
		Last Modified: Thu, 06 May 2021 19:17:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9cc492f2ab4768092dd4ee65dda48b96ba0b078d873324033e9f78f143c3f`  
		Last Modified: Fri, 07 May 2021 01:19:53 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:51771aedb5d0131042e775e300f8a6a2e266e30f9bf913680ecdca30e9c2390c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:f16d74a62cf3f36dc0ac5167cbe244aeea0f86fdda9436815f3b3f972d6142b8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762028419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3558140470646ef42a86763f4b03a4309b61d072624f02db29c4bb8d8074b603`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:17:45 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:17:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:17:51 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:21:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:21:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:21:56 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:21:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5084dad826c0c649041897fde59f2f8a29657aa36c87dd0ca01f8378e2ac09`  
		Last Modified: Wed, 12 May 2021 00:50:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497aaa432c047dc516f3c3746627b20f533ef1d3f326d30ea81ff17b862cb76`  
		Last Modified: Wed, 12 May 2021 00:50:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a6d0366ca7a4a28b6b3e907dd88321d0b99d180fe40e46823196b1a5660849`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bc979d308d872e587349eb82ed7c3deca66071069c720289c500958a66fd37`  
		Last Modified: Wed, 12 May 2021 00:51:52 GMT  
		Size: 287.5 MB (287529301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2206506a92dd9bb5e31fd2690a0587bf9b991a7fff77a8adf8debed039a06e6c`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5721150e73a1b0b3fda4086694b5ae65dde321f33568ed2ede9181b4e5ec709b`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced697788b22eeb4cc380add1d86cf0e529eff5166667d0bb7ea1e2978344544`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:7afa0ae0c26ab1fc0de929d6db3c346fb460ee5340f37d9d5ef8075009d1ab81
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088400521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92591f36b34947f6d14367125172e6237635b79a73fd82dc0674aed20d50202`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:22:19 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:22:21 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:22:24 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:28:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:28:12 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:28:14 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:28:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64101d9b7b40bb5c07101ee6fe77973e5f71d74067f4fca6c64f66423e12ec`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775b49a444eb1bf0c1179a704f2f8cb229c0e7d4cc6d3cdcd098de593a7c9455`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21c661196aed0c6d9d732de3fcda2f079cc3a018f81c2f23c9437333a9c807`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b3290d98042dcbef7e5d2589d8a45dab1f9ef8902a3f2aff55042694c7950`  
		Last Modified: Wed, 12 May 2021 00:53:12 GMT  
		Size: 292.6 MB (292613155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186bb0a3b7d0556de16f08bb4fff7502c052527541f637637db3d9b4fb39abc`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5399e68624877eb89ac01abbe8edf59e0126b9100e65cb25306e495dc0ca2150`  
		Last Modified: Wed, 12 May 2021 00:52:07 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3112946af906f623bc85ba3e6feb706023451eae47c618b8a861d21fcd34e9`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:de342cbae19f35a0a9468d28bfd06ff00f0f8d6b78768e304848c7fea7a36d71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:f16d74a62cf3f36dc0ac5167cbe244aeea0f86fdda9436815f3b3f972d6142b8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762028419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3558140470646ef42a86763f4b03a4309b61d072624f02db29c4bb8d8074b603`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:17:45 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:17:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:17:51 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:21:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:21:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:21:56 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:21:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5084dad826c0c649041897fde59f2f8a29657aa36c87dd0ca01f8378e2ac09`  
		Last Modified: Wed, 12 May 2021 00:50:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497aaa432c047dc516f3c3746627b20f533ef1d3f326d30ea81ff17b862cb76`  
		Last Modified: Wed, 12 May 2021 00:50:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a6d0366ca7a4a28b6b3e907dd88321d0b99d180fe40e46823196b1a5660849`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bc979d308d872e587349eb82ed7c3deca66071069c720289c500958a66fd37`  
		Last Modified: Wed, 12 May 2021 00:51:52 GMT  
		Size: 287.5 MB (287529301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2206506a92dd9bb5e31fd2690a0587bf9b991a7fff77a8adf8debed039a06e6c`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5721150e73a1b0b3fda4086694b5ae65dde321f33568ed2ede9181b4e5ec709b`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced697788b22eeb4cc380add1d86cf0e529eff5166667d0bb7ea1e2978344544`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:d3ed16a333f97eaa285be3466caaf6aad20a5c5c63566e58be586bfcf47a2cae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:7afa0ae0c26ab1fc0de929d6db3c346fb460ee5340f37d9d5ef8075009d1ab81
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088400521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92591f36b34947f6d14367125172e6237635b79a73fd82dc0674aed20d50202`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:22:19 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:22:21 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:22:24 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:28:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:28:12 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:28:14 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:28:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64101d9b7b40bb5c07101ee6fe77973e5f71d74067f4fca6c64f66423e12ec`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775b49a444eb1bf0c1179a704f2f8cb229c0e7d4cc6d3cdcd098de593a7c9455`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21c661196aed0c6d9d732de3fcda2f079cc3a018f81c2f23c9437333a9c807`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b3290d98042dcbef7e5d2589d8a45dab1f9ef8902a3f2aff55042694c7950`  
		Last Modified: Wed, 12 May 2021 00:53:12 GMT  
		Size: 292.6 MB (292613155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186bb0a3b7d0556de16f08bb4fff7502c052527541f637637db3d9b4fb39abc`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5399e68624877eb89ac01abbe8edf59e0126b9100e65cb25306e495dc0ca2150`  
		Last Modified: Wed, 12 May 2021 00:52:07 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3112946af906f623bc85ba3e6feb706023451eae47c618b8a861d21fcd34e9`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.14`

```console
$ docker pull mongo@sha256:5c3059c8191861aaf766ce1ac592ebb42ea71ff13951701049bca93e8d614f96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.2.14` - linux; amd64

```console
$ docker pull mongo@sha256:641c065374d80202ef8ca35c6685832ff08feab9373728fe10038af85aefc645
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165072113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc77715107a90808446742859973f659a3328a979c9d5f420267ecc27353d7b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:29 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 24 Apr 2021 00:41:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:41:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:41:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:41:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:41:31 GMT
ENV MONGO_MAJOR=4.2
# Thu, 06 May 2021 21:19:37 GMT
ENV MONGO_VERSION=4.2.14
# Thu, 06 May 2021 21:19:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 06 May 2021 21:20:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 06 May 2021 21:20:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 06 May 2021 21:20:22 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:23 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:23 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e22c3240221da2469e6e3cc16eea1d29eb13c4bd9cf2fc47603c8b2aed76bf9`  
		Last Modified: Sat, 24 Apr 2021 00:43:49 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30a5431c1beafcc66aea5e2b40a4563110db168246de911f887088d1bffb074`  
		Last Modified: Thu, 06 May 2021 21:21:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a8fafb4cd8e24a41a87c2a38a0834d2448d6f48d1adacd89063360fa3beeb5`  
		Last Modified: Thu, 06 May 2021 21:21:28 GMT  
		Size: 129.6 MB (129556866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e86f8d8fafd6007157f60c327ca170ea84102643514aae6c543be5a70eb6d8`  
		Last Modified: Thu, 06 May 2021 21:21:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c56df947a8a8f46909dc1b87c276ea136819a33f08b63f0f63ea7e61789e00e`  
		Last Modified: Thu, 06 May 2021 23:36:19 GMT  
		Size: 4.5 KB (4476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.14` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:79be37da4cc14b5b16baa1cab614bfa5e9b716994cf37a7b02f877429d924efc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155087094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e99546a4b825ada2a61c060757d85930f463c815086cd80bc6888f838a5aef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:51:43 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 24 Apr 2021 01:51:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:51:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:51:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:51:56 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:51:58 GMT
ENV MONGO_MAJOR=4.2
# Thu, 06 May 2021 19:15:43 GMT
ENV MONGO_VERSION=4.2.14
# Thu, 06 May 2021 19:15:47 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 06 May 2021 19:16:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 06 May 2021 19:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 06 May 2021 19:16:25 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:19:02 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:19:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:19:04 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:19:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e8f8e5e40c62eec6f8ce68e5746d9f4fbaab0274a2f613e2f1d5f7439050e`  
		Last Modified: Sat, 24 Apr 2021 01:55:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9d41cfdf0739861bf0e4c14df5e93bbaa099e91a6cc2b7216f8aebb927cb36`  
		Last Modified: Thu, 06 May 2021 19:17:06 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d29221a58b621dd1174f266c393ca3cc0f41514bd78d636080be446730fe3`  
		Last Modified: Thu, 06 May 2021 19:17:31 GMT  
		Size: 123.4 MB (123357635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47de4b46f14ac681b5b70ec05b23c320169f35b243defe2ac4989706bde1fd`  
		Last Modified: Thu, 06 May 2021 19:17:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9cc492f2ab4768092dd4ee65dda48b96ba0b078d873324033e9f78f143c3f`  
		Last Modified: Fri, 07 May 2021 01:19:53 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.14` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:f16d74a62cf3f36dc0ac5167cbe244aeea0f86fdda9436815f3b3f972d6142b8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762028419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3558140470646ef42a86763f4b03a4309b61d072624f02db29c4bb8d8074b603`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:17:45 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:17:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:17:51 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:21:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:21:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:21:56 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:21:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5084dad826c0c649041897fde59f2f8a29657aa36c87dd0ca01f8378e2ac09`  
		Last Modified: Wed, 12 May 2021 00:50:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497aaa432c047dc516f3c3746627b20f533ef1d3f326d30ea81ff17b862cb76`  
		Last Modified: Wed, 12 May 2021 00:50:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a6d0366ca7a4a28b6b3e907dd88321d0b99d180fe40e46823196b1a5660849`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bc979d308d872e587349eb82ed7c3deca66071069c720289c500958a66fd37`  
		Last Modified: Wed, 12 May 2021 00:51:52 GMT  
		Size: 287.5 MB (287529301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2206506a92dd9bb5e31fd2690a0587bf9b991a7fff77a8adf8debed039a06e6c`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5721150e73a1b0b3fda4086694b5ae65dde321f33568ed2ede9181b4e5ec709b`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced697788b22eeb4cc380add1d86cf0e529eff5166667d0bb7ea1e2978344544`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.14` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:7afa0ae0c26ab1fc0de929d6db3c346fb460ee5340f37d9d5ef8075009d1ab81
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088400521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92591f36b34947f6d14367125172e6237635b79a73fd82dc0674aed20d50202`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:22:19 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:22:21 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:22:24 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:28:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:28:12 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:28:14 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:28:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64101d9b7b40bb5c07101ee6fe77973e5f71d74067f4fca6c64f66423e12ec`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775b49a444eb1bf0c1179a704f2f8cb229c0e7d4cc6d3cdcd098de593a7c9455`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21c661196aed0c6d9d732de3fcda2f079cc3a018f81c2f23c9437333a9c807`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b3290d98042dcbef7e5d2589d8a45dab1f9ef8902a3f2aff55042694c7950`  
		Last Modified: Wed, 12 May 2021 00:53:12 GMT  
		Size: 292.6 MB (292613155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186bb0a3b7d0556de16f08bb4fff7502c052527541f637637db3d9b4fb39abc`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5399e68624877eb89ac01abbe8edf59e0126b9100e65cb25306e495dc0ca2150`  
		Last Modified: Wed, 12 May 2021 00:52:07 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3112946af906f623bc85ba3e6feb706023451eae47c618b8a861d21fcd34e9`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.14-bionic`

```console
$ docker pull mongo@sha256:d5b168f0e913255d0383fad82222f314cc1f6253add9c8bdbdac11aecabccf7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2.14-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:641c065374d80202ef8ca35c6685832ff08feab9373728fe10038af85aefc645
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165072113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc77715107a90808446742859973f659a3328a979c9d5f420267ecc27353d7b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:29 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 24 Apr 2021 00:41:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:41:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:41:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:41:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:41:31 GMT
ENV MONGO_MAJOR=4.2
# Thu, 06 May 2021 21:19:37 GMT
ENV MONGO_VERSION=4.2.14
# Thu, 06 May 2021 21:19:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 06 May 2021 21:20:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 06 May 2021 21:20:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 06 May 2021 21:20:22 GMT
VOLUME [/data/db /data/configdb]
# Thu, 06 May 2021 23:35:23 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 06 May 2021 23:35:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 May 2021 23:35:23 GMT
EXPOSE 27017
# Thu, 06 May 2021 23:35:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e22c3240221da2469e6e3cc16eea1d29eb13c4bd9cf2fc47603c8b2aed76bf9`  
		Last Modified: Sat, 24 Apr 2021 00:43:49 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30a5431c1beafcc66aea5e2b40a4563110db168246de911f887088d1bffb074`  
		Last Modified: Thu, 06 May 2021 21:21:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a8fafb4cd8e24a41a87c2a38a0834d2448d6f48d1adacd89063360fa3beeb5`  
		Last Modified: Thu, 06 May 2021 21:21:28 GMT  
		Size: 129.6 MB (129556866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e86f8d8fafd6007157f60c327ca170ea84102643514aae6c543be5a70eb6d8`  
		Last Modified: Thu, 06 May 2021 21:21:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c56df947a8a8f46909dc1b87c276ea136819a33f08b63f0f63ea7e61789e00e`  
		Last Modified: Thu, 06 May 2021 23:36:19 GMT  
		Size: 4.5 KB (4476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.14-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:79be37da4cc14b5b16baa1cab614bfa5e9b716994cf37a7b02f877429d924efc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155087094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e99546a4b825ada2a61c060757d85930f463c815086cd80bc6888f838a5aef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:51:43 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 24 Apr 2021 01:51:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:51:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:51:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:51:56 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:51:58 GMT
ENV MONGO_MAJOR=4.2
# Thu, 06 May 2021 19:15:43 GMT
ENV MONGO_VERSION=4.2.14
# Thu, 06 May 2021 19:15:47 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 06 May 2021 19:16:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 06 May 2021 19:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 06 May 2021 19:16:25 GMT
VOLUME [/data/db /data/configdb]
# Fri, 07 May 2021 01:19:02 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Fri, 07 May 2021 01:19:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 01:19:04 GMT
EXPOSE 27017
# Fri, 07 May 2021 01:19:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e8f8e5e40c62eec6f8ce68e5746d9f4fbaab0274a2f613e2f1d5f7439050e`  
		Last Modified: Sat, 24 Apr 2021 01:55:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9d41cfdf0739861bf0e4c14df5e93bbaa099e91a6cc2b7216f8aebb927cb36`  
		Last Modified: Thu, 06 May 2021 19:17:06 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d29221a58b621dd1174f266c393ca3cc0f41514bd78d636080be446730fe3`  
		Last Modified: Thu, 06 May 2021 19:17:31 GMT  
		Size: 123.4 MB (123357635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47de4b46f14ac681b5b70ec05b23c320169f35b243defe2ac4989706bde1fd`  
		Last Modified: Thu, 06 May 2021 19:17:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9cc492f2ab4768092dd4ee65dda48b96ba0b078d873324033e9f78f143c3f`  
		Last Modified: Fri, 07 May 2021 01:19:53 GMT  
		Size: 4.5 KB (4470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.14-windowsservercore`

```console
$ docker pull mongo@sha256:51771aedb5d0131042e775e300f8a6a2e266e30f9bf913680ecdca30e9c2390c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.2.14-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:f16d74a62cf3f36dc0ac5167cbe244aeea0f86fdda9436815f3b3f972d6142b8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762028419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3558140470646ef42a86763f4b03a4309b61d072624f02db29c4bb8d8074b603`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:17:45 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:17:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:17:51 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:21:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:21:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:21:56 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:21:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5084dad826c0c649041897fde59f2f8a29657aa36c87dd0ca01f8378e2ac09`  
		Last Modified: Wed, 12 May 2021 00:50:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497aaa432c047dc516f3c3746627b20f533ef1d3f326d30ea81ff17b862cb76`  
		Last Modified: Wed, 12 May 2021 00:50:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a6d0366ca7a4a28b6b3e907dd88321d0b99d180fe40e46823196b1a5660849`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bc979d308d872e587349eb82ed7c3deca66071069c720289c500958a66fd37`  
		Last Modified: Wed, 12 May 2021 00:51:52 GMT  
		Size: 287.5 MB (287529301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2206506a92dd9bb5e31fd2690a0587bf9b991a7fff77a8adf8debed039a06e6c`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5721150e73a1b0b3fda4086694b5ae65dde321f33568ed2ede9181b4e5ec709b`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced697788b22eeb4cc380add1d86cf0e529eff5166667d0bb7ea1e2978344544`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.14-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:7afa0ae0c26ab1fc0de929d6db3c346fb460ee5340f37d9d5ef8075009d1ab81
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088400521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92591f36b34947f6d14367125172e6237635b79a73fd82dc0674aed20d50202`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:22:19 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:22:21 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:22:24 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:28:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:28:12 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:28:14 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:28:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64101d9b7b40bb5c07101ee6fe77973e5f71d74067f4fca6c64f66423e12ec`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775b49a444eb1bf0c1179a704f2f8cb229c0e7d4cc6d3cdcd098de593a7c9455`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21c661196aed0c6d9d732de3fcda2f079cc3a018f81c2f23c9437333a9c807`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b3290d98042dcbef7e5d2589d8a45dab1f9ef8902a3f2aff55042694c7950`  
		Last Modified: Wed, 12 May 2021 00:53:12 GMT  
		Size: 292.6 MB (292613155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186bb0a3b7d0556de16f08bb4fff7502c052527541f637637db3d9b4fb39abc`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5399e68624877eb89ac01abbe8edf59e0126b9100e65cb25306e495dc0ca2150`  
		Last Modified: Wed, 12 May 2021 00:52:07 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3112946af906f623bc85ba3e6feb706023451eae47c618b8a861d21fcd34e9`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.14-windowsservercore-1809`

```console
$ docker pull mongo@sha256:de342cbae19f35a0a9468d28bfd06ff00f0f8d6b78768e304848c7fea7a36d71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:4.2.14-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:f16d74a62cf3f36dc0ac5167cbe244aeea0f86fdda9436815f3b3f972d6142b8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762028419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3558140470646ef42a86763f4b03a4309b61d072624f02db29c4bb8d8074b603`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:17:45 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:17:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:17:51 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:21:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:21:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:21:56 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:21:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5084dad826c0c649041897fde59f2f8a29657aa36c87dd0ca01f8378e2ac09`  
		Last Modified: Wed, 12 May 2021 00:50:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497aaa432c047dc516f3c3746627b20f533ef1d3f326d30ea81ff17b862cb76`  
		Last Modified: Wed, 12 May 2021 00:50:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a6d0366ca7a4a28b6b3e907dd88321d0b99d180fe40e46823196b1a5660849`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bc979d308d872e587349eb82ed7c3deca66071069c720289c500958a66fd37`  
		Last Modified: Wed, 12 May 2021 00:51:52 GMT  
		Size: 287.5 MB (287529301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2206506a92dd9bb5e31fd2690a0587bf9b991a7fff77a8adf8debed039a06e6c`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5721150e73a1b0b3fda4086694b5ae65dde321f33568ed2ede9181b4e5ec709b`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced697788b22eeb4cc380add1d86cf0e529eff5166667d0bb7ea1e2978344544`  
		Last Modified: Wed, 12 May 2021 00:50:49 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.14-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:d3ed16a333f97eaa285be3466caaf6aad20a5c5c63566e58be586bfcf47a2cae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.2.14-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:7afa0ae0c26ab1fc0de929d6db3c346fb460ee5340f37d9d5ef8075009d1ab81
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088400521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92591f36b34947f6d14367125172e6237635b79a73fd82dc0674aed20d50202`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:22:19 GMT
ENV MONGO_VERSION=4.2.14
# Wed, 12 May 2021 00:22:21 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.14-signed.msi
# Wed, 12 May 2021 00:22:24 GMT
ENV MONGO_DOWNLOAD_SHA256=706610f96ae74963d5348aafe34f976e7b1c02ef1a9f3596862e1e5ba3437e76
# Wed, 12 May 2021 00:28:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:28:12 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:28:14 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:28:16 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64101d9b7b40bb5c07101ee6fe77973e5f71d74067f4fca6c64f66423e12ec`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775b49a444eb1bf0c1179a704f2f8cb229c0e7d4cc6d3cdcd098de593a7c9455`  
		Last Modified: Wed, 12 May 2021 00:52:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21c661196aed0c6d9d732de3fcda2f079cc3a018f81c2f23c9437333a9c807`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b3290d98042dcbef7e5d2589d8a45dab1f9ef8902a3f2aff55042694c7950`  
		Last Modified: Wed, 12 May 2021 00:53:12 GMT  
		Size: 292.6 MB (292613155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186bb0a3b7d0556de16f08bb4fff7502c052527541f637637db3d9b4fb39abc`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5399e68624877eb89ac01abbe8edf59e0126b9100e65cb25306e495dc0ca2150`  
		Last Modified: Wed, 12 May 2021 00:52:07 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3112946af906f623bc85ba3e6feb706023451eae47c618b8a861d21fcd34e9`  
		Last Modified: Wed, 12 May 2021 00:52:06 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4`

```console
$ docker pull mongo@sha256:401ae88210c708d54873af22df618b46a5f3d2da1c2676d115326b205ec78d3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.4` - linux; amd64

```console
$ docker pull mongo@sha256:ebb6b8403c1f47069b099f1ba75778d41e15a5d8eed3db6f435733333e403a2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175677269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07630e791de3ceb87d39543799438e118753246d19dcfd6529bd4d27ff1b83bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:58 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 00:41:59 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:11:00 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:11:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:11:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:11:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:11:48 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:11:49 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:11:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:11:49 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:11:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2ff17242ce7e307fbd191a597f210061566606443ff6632ca685d394cb9acf`  
		Last Modified: Sat, 24 Apr 2021 00:44:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11b2ce05942f19ca819aa8c130575b0850153384fba7f489fd1a62ec0d94e7`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91532386f4ec7af743bc43ddbab8410d9d2fee68ce63bca3aa397c04e29b9091`  
		Last Modified: Tue, 11 May 2021 00:12:51 GMT  
		Size: 140.2 MB (140162019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705ef0ab262e766f32008195b4e3719f5444b83e3218dbab09f5cfa7098322ea`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6238126b609f01bb47ddd8598f331bb5cb7653f2d9798eb2f14d48061d8e279`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 4.5 KB (4477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8f2c9016beb50c2972e54c732d8dc24fb332360104b9e71767af9c4e71c1348e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168070890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3a757873434f9961cb2b732f35c712866d65e5fdf009c9b8572d46c0657e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 01:53:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:53:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:08 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 01:41:03 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 01:41:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 01:41:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 01:41:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 01:41:41 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 01:41:42 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 01:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:41:44 GMT
EXPOSE 27017
# Tue, 11 May 2021 01:41:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b8f707197ef2788f2ed0cf82b088b9262efb9b7a374da64bb70daccca6525`  
		Last Modified: Sat, 24 Apr 2021 01:56:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d9f84ef7c607013458b7c4f0045d42081a3cd4e32e09a99c45af7af1742eb`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a71fa0bced6eaef2a94dfda7f28a3c97b1f52e0def1e877932edf84e97df5`  
		Last Modified: Tue, 11 May 2021 01:42:41 GMT  
		Size: 136.3 MB (136341433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88698b947abf4aa832fdbc0c629195e7b8ad1790baad6dfa6ad42b0201e5b81e`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7dfc922696b1eae0c53f3c4559bdfca5ae0dd740a6c3e5166c0839e4ce49ad`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; s390x

```console
$ docker pull mongo@sha256:c8e981f281462baf0c84890eab82c4fad6c825d221664b463ccd43485f6380cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169474559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8b1f024425214a141ef62568a875dc3f443453094dbe43757c3a42d5ada69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:51:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Apr 2021 22:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:51:56 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 22:51:57 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Apr 2021 22:52:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 22:52:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 22:52:19 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 23 Apr 2021 22:52:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:24 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:38:53 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:38:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:39:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:39:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:39:55 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:39:55 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:39:56 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:39:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bc20f34c3c0e6defa11123a46488ad9866f1cbed77d74904f7b057f014902`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934bd72760b936ef87cda05b4fd31a1266859e77f6960e8b6a17eb4df55b82b2`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 2.7 MB (2708330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778576254d798d87ee503dd46947744945440e160227cf20f86506eb7f0c752`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 5.7 MB (5747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b7218def3876e2bd7ede8db669dd67c94e3f67db5c8b385e7d0b189c70f19`  
		Last Modified: Fri, 23 Apr 2021 22:53:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218c55b05ae6da8d768db66caf009228dd32c56943df536e02932cd24a359f1e`  
		Last Modified: Fri, 23 Apr 2021 22:53:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921db7ddca2b72930c0ba65cfcf991843ce2fdee70e5ed022876b6f5bebbe5`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c499f2e405c30092431c8a9e2734154a24af4ed421ff0c7d97b16d1b02f39`  
		Last Modified: Tue, 11 May 2021 00:40:40 GMT  
		Size: 135.7 MB (135656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1d700e09af9f173c1ca948355e0d1a01b5c6139b36889ca0621055669821f9`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99d8d95772dfd5147e631e7e072172ebe7c33d5d8916e8f372607a7c866572`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:8027a70fbe7e47adb3b0970eacbbc1dd78cf06203cf320da5cdbc5cf71d3e01d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037334566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35400f2fef53c6fde1a596644884d280e42c2043b303fb8a64bf09ddebe3d0b5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:33:49 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:33:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:33:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:39:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:39:49 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:39:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa26c3b7dd5be40e6af6e110598ff8ade5597433a780e713fe02d41a01ff4ab`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcc96fa02f1eff07ba750778c31dbc2a2b2eb1205d0862a2ebe6b93c8f2785b`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264615459bc5dd410e8fdba7e066381e9fd687efbafbcbdc04d6a3c8f19ccb5`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93394405d931bc35ec98aec50a2d8664f5c0580f16dbae47c70dabbebf81356d`  
		Last Modified: Wed, 12 May 2021 00:59:03 GMT  
		Size: 241.5 MB (241547428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4854c02134142d249afb7fb7045fd09f266e95fce580e919b709b8dac5572bc`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea254f563aa38c2c7a29f573537255e55d3b9e8ab8c43bd857e1e8ea156bb9c4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0592557aaf1bfb0d38c61451aa21ccc7d3b5e447d85f6e38b920c27ebc0eb7b4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-bionic`

```console
$ docker pull mongo@sha256:3dbb3b4b8f33c8a61fa72cf1d05398d6cc09c72aa2a1f664b639d8231b0e83ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:ebb6b8403c1f47069b099f1ba75778d41e15a5d8eed3db6f435733333e403a2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175677269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07630e791de3ceb87d39543799438e118753246d19dcfd6529bd4d27ff1b83bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:58 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 00:41:59 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:11:00 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:11:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:11:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:11:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:11:48 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:11:49 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:11:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:11:49 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:11:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2ff17242ce7e307fbd191a597f210061566606443ff6632ca685d394cb9acf`  
		Last Modified: Sat, 24 Apr 2021 00:44:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11b2ce05942f19ca819aa8c130575b0850153384fba7f489fd1a62ec0d94e7`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91532386f4ec7af743bc43ddbab8410d9d2fee68ce63bca3aa397c04e29b9091`  
		Last Modified: Tue, 11 May 2021 00:12:51 GMT  
		Size: 140.2 MB (140162019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705ef0ab262e766f32008195b4e3719f5444b83e3218dbab09f5cfa7098322ea`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6238126b609f01bb47ddd8598f331bb5cb7653f2d9798eb2f14d48061d8e279`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 4.5 KB (4477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8f2c9016beb50c2972e54c732d8dc24fb332360104b9e71767af9c4e71c1348e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168070890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3a757873434f9961cb2b732f35c712866d65e5fdf009c9b8572d46c0657e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 01:53:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:53:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:08 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 01:41:03 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 01:41:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 01:41:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 01:41:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 01:41:41 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 01:41:42 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 01:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:41:44 GMT
EXPOSE 27017
# Tue, 11 May 2021 01:41:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b8f707197ef2788f2ed0cf82b088b9262efb9b7a374da64bb70daccca6525`  
		Last Modified: Sat, 24 Apr 2021 01:56:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d9f84ef7c607013458b7c4f0045d42081a3cd4e32e09a99c45af7af1742eb`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a71fa0bced6eaef2a94dfda7f28a3c97b1f52e0def1e877932edf84e97df5`  
		Last Modified: Tue, 11 May 2021 01:42:41 GMT  
		Size: 136.3 MB (136341433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88698b947abf4aa832fdbc0c629195e7b8ad1790baad6dfa6ad42b0201e5b81e`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7dfc922696b1eae0c53f3c4559bdfca5ae0dd740a6c3e5166c0839e4ce49ad`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:c8e981f281462baf0c84890eab82c4fad6c825d221664b463ccd43485f6380cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169474559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8b1f024425214a141ef62568a875dc3f443453094dbe43757c3a42d5ada69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:51:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Apr 2021 22:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:51:56 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 22:51:57 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Apr 2021 22:52:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 22:52:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 22:52:19 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 23 Apr 2021 22:52:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:24 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:38:53 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:38:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:39:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:39:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:39:55 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:39:55 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:39:56 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:39:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bc20f34c3c0e6defa11123a46488ad9866f1cbed77d74904f7b057f014902`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934bd72760b936ef87cda05b4fd31a1266859e77f6960e8b6a17eb4df55b82b2`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 2.7 MB (2708330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778576254d798d87ee503dd46947744945440e160227cf20f86506eb7f0c752`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 5.7 MB (5747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b7218def3876e2bd7ede8db669dd67c94e3f67db5c8b385e7d0b189c70f19`  
		Last Modified: Fri, 23 Apr 2021 22:53:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218c55b05ae6da8d768db66caf009228dd32c56943df536e02932cd24a359f1e`  
		Last Modified: Fri, 23 Apr 2021 22:53:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921db7ddca2b72930c0ba65cfcf991843ce2fdee70e5ed022876b6f5bebbe5`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c499f2e405c30092431c8a9e2734154a24af4ed421ff0c7d97b16d1b02f39`  
		Last Modified: Tue, 11 May 2021 00:40:40 GMT  
		Size: 135.7 MB (135656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1d700e09af9f173c1ca948355e0d1a01b5c6139b36889ca0621055669821f9`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99d8d95772dfd5147e631e7e072172ebe7c33d5d8916e8f372607a7c866572`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore`

```console
$ docker pull mongo@sha256:eb0c7d46164fd225423e2c0fc64e96f52c38b738f8fd9ccba13e56c4eb119275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `mongo:4.4-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull mongo@sha256:e2dc6e2ce10059a0d52f2e7ef003b495ed57e72c0b0e00bac2148b20dec63355
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706212737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ddc9cab99b833b8495cc7ee447d7c65463a6c877af4d80d4aa833b6d64b99a5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 10 May 2021 23:15:58 GMT
ENV MONGO_VERSION=4.4.6
# Mon, 10 May 2021 23:15:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Mon, 10 May 2021 23:16:01 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Mon, 10 May 2021 23:18:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 10 May 2021 23:18:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 10 May 2021 23:18:25 GMT
EXPOSE 27017
# Mon, 10 May 2021 23:18:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1af6a38cdaf02b9763a51588fe3ec107b6324e3c240b81be1c53374619c675`  
		Last Modified: Mon, 10 May 2021 23:24:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4550f7fa25bb90c099b1eac08fa398f54f44d40adeb082ad7c38a62223c6a411`  
		Last Modified: Mon, 10 May 2021 23:24:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdfb1c878583e1857a026502bc1d5644702990001c8ed20f4b1b647706c59b`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417a1588a5fc27f1d60b2a2ea14002824a5de37b9d3ad7ccbb2484e44c3a9dcf`  
		Last Modified: Mon, 10 May 2021 23:24:48 GMT  
		Size: 236.4 MB (236448794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed7b32008983c9797db237aa9a90c851d502b47467b518ec9060f17065ca44`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b56283a6d31ef57873809be37e8516d0606ab794493b8237b90eb5b91be6b2`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb68b8b769ff2ae29874c729c09a2db8d3e7e0727b7b486792074d26ff7d802`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull mongo@sha256:2eac7d1f71ed080a26b742240fe92543fe2e940bb5a48fdd59ac3fecc0e9e73c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6036382733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03eb8c7454248dc61a5ae434a904103696979b3e44430a44cedeb70ec3b92a7a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 10 May 2021 23:18:41 GMT
ENV MONGO_VERSION=4.4.6
# Mon, 10 May 2021 23:18:43 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Mon, 10 May 2021 23:18:44 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Mon, 10 May 2021 23:22:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 10 May 2021 23:22:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 10 May 2021 23:22:16 GMT
EXPOSE 27017
# Mon, 10 May 2021 23:22:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b78e3aa88d4e50d3d51ac081c91eeef9933d4a7a75f4845821519ed2bd1a3`  
		Last Modified: Mon, 10 May 2021 23:25:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f41596dd2dda6342571328e8de671fc73c58da781f443547f9bd94b2e602a1a`  
		Last Modified: Mon, 10 May 2021 23:25:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0fd0da468dbf2b3fb5817a9dfe9badc42a5ae933fe238ba533b51dcd548b8`  
		Last Modified: Mon, 10 May 2021 23:25:06 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228c37f48edb438de1305cde961522a16d6041442f1b377b315370fad7c041c`  
		Last Modified: Mon, 10 May 2021 23:26:04 GMT  
		Size: 241.5 MB (241488971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94206c6a1738fc370c80eb4e0259a1a74df12b0c8fa4fd45227cbd18d38bbf1`  
		Last Modified: Mon, 10 May 2021 23:25:05 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4cfcf8250b04c427f36ba05bef1ef1e42cb65e92b9f3cc2fd3f3c4fc976c65`  
		Last Modified: Mon, 10 May 2021 23:25:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0f9cb3fef403e1662a10830f0d076d9cdd0d374fd01875379380b862a41009`  
		Last Modified: Mon, 10 May 2021 23:25:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:8917c43037c70887cbb4140acc128cea9c1c2fd7fcb70257d20145baedbd6fab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:4.4-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:c1c7f59a7f29591106d067877ad4e568d260572adcd9803d1fef162ca4ec9a22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:8027a70fbe7e47adb3b0970eacbbc1dd78cf06203cf320da5cdbc5cf71d3e01d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037334566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35400f2fef53c6fde1a596644884d280e42c2043b303fb8a64bf09ddebe3d0b5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:33:49 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:33:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:33:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:39:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:39:49 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:39:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa26c3b7dd5be40e6af6e110598ff8ade5597433a780e713fe02d41a01ff4ab`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcc96fa02f1eff07ba750778c31dbc2a2b2eb1205d0862a2ebe6b93c8f2785b`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264615459bc5dd410e8fdba7e066381e9fd687efbafbcbdc04d6a3c8f19ccb5`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93394405d931bc35ec98aec50a2d8664f5c0580f16dbae47c70dabbebf81356d`  
		Last Modified: Wed, 12 May 2021 00:59:03 GMT  
		Size: 241.5 MB (241547428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4854c02134142d249afb7fb7045fd09f266e95fce580e919b709b8dac5572bc`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea254f563aa38c2c7a29f573537255e55d3b9e8ab8c43bd857e1e8ea156bb9c4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0592557aaf1bfb0d38c61451aa21ccc7d3b5e447d85f6e38b920c27ebc0eb7b4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.6`

```console
$ docker pull mongo@sha256:401ae88210c708d54873af22df618b46a5f3d2da1c2676d115326b205ec78d3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.4.6` - linux; amd64

```console
$ docker pull mongo@sha256:ebb6b8403c1f47069b099f1ba75778d41e15a5d8eed3db6f435733333e403a2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175677269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07630e791de3ceb87d39543799438e118753246d19dcfd6529bd4d27ff1b83bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:58 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 00:41:59 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:11:00 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:11:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:11:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:11:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:11:48 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:11:49 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:11:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:11:49 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:11:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2ff17242ce7e307fbd191a597f210061566606443ff6632ca685d394cb9acf`  
		Last Modified: Sat, 24 Apr 2021 00:44:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11b2ce05942f19ca819aa8c130575b0850153384fba7f489fd1a62ec0d94e7`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91532386f4ec7af743bc43ddbab8410d9d2fee68ce63bca3aa397c04e29b9091`  
		Last Modified: Tue, 11 May 2021 00:12:51 GMT  
		Size: 140.2 MB (140162019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705ef0ab262e766f32008195b4e3719f5444b83e3218dbab09f5cfa7098322ea`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6238126b609f01bb47ddd8598f331bb5cb7653f2d9798eb2f14d48061d8e279`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 4.5 KB (4477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8f2c9016beb50c2972e54c732d8dc24fb332360104b9e71767af9c4e71c1348e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168070890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3a757873434f9961cb2b732f35c712866d65e5fdf009c9b8572d46c0657e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 01:53:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:53:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:08 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 01:41:03 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 01:41:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 01:41:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 01:41:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 01:41:41 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 01:41:42 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 01:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:41:44 GMT
EXPOSE 27017
# Tue, 11 May 2021 01:41:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b8f707197ef2788f2ed0cf82b088b9262efb9b7a374da64bb70daccca6525`  
		Last Modified: Sat, 24 Apr 2021 01:56:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d9f84ef7c607013458b7c4f0045d42081a3cd4e32e09a99c45af7af1742eb`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a71fa0bced6eaef2a94dfda7f28a3c97b1f52e0def1e877932edf84e97df5`  
		Last Modified: Tue, 11 May 2021 01:42:41 GMT  
		Size: 136.3 MB (136341433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88698b947abf4aa832fdbc0c629195e7b8ad1790baad6dfa6ad42b0201e5b81e`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7dfc922696b1eae0c53f3c4559bdfca5ae0dd740a6c3e5166c0839e4ce49ad`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.6` - linux; s390x

```console
$ docker pull mongo@sha256:c8e981f281462baf0c84890eab82c4fad6c825d221664b463ccd43485f6380cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169474559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8b1f024425214a141ef62568a875dc3f443453094dbe43757c3a42d5ada69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:51:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Apr 2021 22:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:51:56 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 22:51:57 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Apr 2021 22:52:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 22:52:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 22:52:19 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 23 Apr 2021 22:52:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:24 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:38:53 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:38:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:39:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:39:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:39:55 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:39:55 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:39:56 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:39:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bc20f34c3c0e6defa11123a46488ad9866f1cbed77d74904f7b057f014902`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934bd72760b936ef87cda05b4fd31a1266859e77f6960e8b6a17eb4df55b82b2`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 2.7 MB (2708330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778576254d798d87ee503dd46947744945440e160227cf20f86506eb7f0c752`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 5.7 MB (5747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b7218def3876e2bd7ede8db669dd67c94e3f67db5c8b385e7d0b189c70f19`  
		Last Modified: Fri, 23 Apr 2021 22:53:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218c55b05ae6da8d768db66caf009228dd32c56943df536e02932cd24a359f1e`  
		Last Modified: Fri, 23 Apr 2021 22:53:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921db7ddca2b72930c0ba65cfcf991843ce2fdee70e5ed022876b6f5bebbe5`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c499f2e405c30092431c8a9e2734154a24af4ed421ff0c7d97b16d1b02f39`  
		Last Modified: Tue, 11 May 2021 00:40:40 GMT  
		Size: 135.7 MB (135656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1d700e09af9f173c1ca948355e0d1a01b5c6139b36889ca0621055669821f9`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99d8d95772dfd5147e631e7e072172ebe7c33d5d8916e8f372607a7c866572`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.6` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.6` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:8027a70fbe7e47adb3b0970eacbbc1dd78cf06203cf320da5cdbc5cf71d3e01d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037334566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35400f2fef53c6fde1a596644884d280e42c2043b303fb8a64bf09ddebe3d0b5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:33:49 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:33:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:33:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:39:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:39:49 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:39:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa26c3b7dd5be40e6af6e110598ff8ade5597433a780e713fe02d41a01ff4ab`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcc96fa02f1eff07ba750778c31dbc2a2b2eb1205d0862a2ebe6b93c8f2785b`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264615459bc5dd410e8fdba7e066381e9fd687efbafbcbdc04d6a3c8f19ccb5`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93394405d931bc35ec98aec50a2d8664f5c0580f16dbae47c70dabbebf81356d`  
		Last Modified: Wed, 12 May 2021 00:59:03 GMT  
		Size: 241.5 MB (241547428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4854c02134142d249afb7fb7045fd09f266e95fce580e919b709b8dac5572bc`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea254f563aa38c2c7a29f573537255e55d3b9e8ab8c43bd857e1e8ea156bb9c4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0592557aaf1bfb0d38c61451aa21ccc7d3b5e447d85f6e38b920c27ebc0eb7b4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.6-bionic`

```console
$ docker pull mongo@sha256:3dbb3b4b8f33c8a61fa72cf1d05398d6cc09c72aa2a1f664b639d8231b0e83ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.6-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:ebb6b8403c1f47069b099f1ba75778d41e15a5d8eed3db6f435733333e403a2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175677269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07630e791de3ceb87d39543799438e118753246d19dcfd6529bd4d27ff1b83bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:58 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 00:41:59 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:11:00 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:11:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:11:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:11:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:11:48 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:11:49 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:11:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:11:49 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:11:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2ff17242ce7e307fbd191a597f210061566606443ff6632ca685d394cb9acf`  
		Last Modified: Sat, 24 Apr 2021 00:44:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11b2ce05942f19ca819aa8c130575b0850153384fba7f489fd1a62ec0d94e7`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91532386f4ec7af743bc43ddbab8410d9d2fee68ce63bca3aa397c04e29b9091`  
		Last Modified: Tue, 11 May 2021 00:12:51 GMT  
		Size: 140.2 MB (140162019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705ef0ab262e766f32008195b4e3719f5444b83e3218dbab09f5cfa7098322ea`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6238126b609f01bb47ddd8598f331bb5cb7653f2d9798eb2f14d48061d8e279`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 4.5 KB (4477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.6-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8f2c9016beb50c2972e54c732d8dc24fb332360104b9e71767af9c4e71c1348e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168070890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3a757873434f9961cb2b732f35c712866d65e5fdf009c9b8572d46c0657e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 01:53:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:53:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:08 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 01:41:03 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 01:41:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 01:41:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 01:41:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 01:41:41 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 01:41:42 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 01:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:41:44 GMT
EXPOSE 27017
# Tue, 11 May 2021 01:41:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b8f707197ef2788f2ed0cf82b088b9262efb9b7a374da64bb70daccca6525`  
		Last Modified: Sat, 24 Apr 2021 01:56:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d9f84ef7c607013458b7c4f0045d42081a3cd4e32e09a99c45af7af1742eb`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a71fa0bced6eaef2a94dfda7f28a3c97b1f52e0def1e877932edf84e97df5`  
		Last Modified: Tue, 11 May 2021 01:42:41 GMT  
		Size: 136.3 MB (136341433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88698b947abf4aa832fdbc0c629195e7b8ad1790baad6dfa6ad42b0201e5b81e`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7dfc922696b1eae0c53f3c4559bdfca5ae0dd740a6c3e5166c0839e4ce49ad`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.6-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:c8e981f281462baf0c84890eab82c4fad6c825d221664b463ccd43485f6380cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169474559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8b1f024425214a141ef62568a875dc3f443453094dbe43757c3a42d5ada69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:51:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Apr 2021 22:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:51:56 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 22:51:57 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Apr 2021 22:52:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 22:52:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 22:52:19 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 23 Apr 2021 22:52:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:24 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:38:53 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:38:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:39:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:39:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:39:55 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:39:55 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:39:56 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:39:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bc20f34c3c0e6defa11123a46488ad9866f1cbed77d74904f7b057f014902`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934bd72760b936ef87cda05b4fd31a1266859e77f6960e8b6a17eb4df55b82b2`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 2.7 MB (2708330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778576254d798d87ee503dd46947744945440e160227cf20f86506eb7f0c752`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 5.7 MB (5747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b7218def3876e2bd7ede8db669dd67c94e3f67db5c8b385e7d0b189c70f19`  
		Last Modified: Fri, 23 Apr 2021 22:53:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218c55b05ae6da8d768db66caf009228dd32c56943df536e02932cd24a359f1e`  
		Last Modified: Fri, 23 Apr 2021 22:53:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921db7ddca2b72930c0ba65cfcf991843ce2fdee70e5ed022876b6f5bebbe5`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c499f2e405c30092431c8a9e2734154a24af4ed421ff0c7d97b16d1b02f39`  
		Last Modified: Tue, 11 May 2021 00:40:40 GMT  
		Size: 135.7 MB (135656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1d700e09af9f173c1ca948355e0d1a01b5c6139b36889ca0621055669821f9`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99d8d95772dfd5147e631e7e072172ebe7c33d5d8916e8f372607a7c866572`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.6-windowsservercore`

```console
$ docker pull mongo@sha256:eb0c7d46164fd225423e2c0fc64e96f52c38b738f8fd9ccba13e56c4eb119275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `mongo:4.4.6-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull mongo@sha256:e2dc6e2ce10059a0d52f2e7ef003b495ed57e72c0b0e00bac2148b20dec63355
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706212737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ddc9cab99b833b8495cc7ee447d7c65463a6c877af4d80d4aa833b6d64b99a5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 10 May 2021 23:15:58 GMT
ENV MONGO_VERSION=4.4.6
# Mon, 10 May 2021 23:15:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Mon, 10 May 2021 23:16:01 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Mon, 10 May 2021 23:18:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 10 May 2021 23:18:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 10 May 2021 23:18:25 GMT
EXPOSE 27017
# Mon, 10 May 2021 23:18:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1af6a38cdaf02b9763a51588fe3ec107b6324e3c240b81be1c53374619c675`  
		Last Modified: Mon, 10 May 2021 23:24:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4550f7fa25bb90c099b1eac08fa398f54f44d40adeb082ad7c38a62223c6a411`  
		Last Modified: Mon, 10 May 2021 23:24:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdfb1c878583e1857a026502bc1d5644702990001c8ed20f4b1b647706c59b`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417a1588a5fc27f1d60b2a2ea14002824a5de37b9d3ad7ccbb2484e44c3a9dcf`  
		Last Modified: Mon, 10 May 2021 23:24:48 GMT  
		Size: 236.4 MB (236448794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed7b32008983c9797db237aa9a90c851d502b47467b518ec9060f17065ca44`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b56283a6d31ef57873809be37e8516d0606ab794493b8237b90eb5b91be6b2`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb68b8b769ff2ae29874c729c09a2db8d3e7e0727b7b486792074d26ff7d802`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.6-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull mongo@sha256:2eac7d1f71ed080a26b742240fe92543fe2e940bb5a48fdd59ac3fecc0e9e73c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6036382733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03eb8c7454248dc61a5ae434a904103696979b3e44430a44cedeb70ec3b92a7a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 10 May 2021 23:18:41 GMT
ENV MONGO_VERSION=4.4.6
# Mon, 10 May 2021 23:18:43 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Mon, 10 May 2021 23:18:44 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Mon, 10 May 2021 23:22:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 10 May 2021 23:22:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 10 May 2021 23:22:16 GMT
EXPOSE 27017
# Mon, 10 May 2021 23:22:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b78e3aa88d4e50d3d51ac081c91eeef9933d4a7a75f4845821519ed2bd1a3`  
		Last Modified: Mon, 10 May 2021 23:25:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f41596dd2dda6342571328e8de671fc73c58da781f443547f9bd94b2e602a1a`  
		Last Modified: Mon, 10 May 2021 23:25:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0fd0da468dbf2b3fb5817a9dfe9badc42a5ae933fe238ba533b51dcd548b8`  
		Last Modified: Mon, 10 May 2021 23:25:06 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228c37f48edb438de1305cde961522a16d6041442f1b377b315370fad7c041c`  
		Last Modified: Mon, 10 May 2021 23:26:04 GMT  
		Size: 241.5 MB (241488971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94206c6a1738fc370c80eb4e0259a1a74df12b0c8fa4fd45227cbd18d38bbf1`  
		Last Modified: Mon, 10 May 2021 23:25:05 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4cfcf8250b04c427f36ba05bef1ef1e42cb65e92b9f3cc2fd3f3c4fc976c65`  
		Last Modified: Mon, 10 May 2021 23:25:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0f9cb3fef403e1662a10830f0d076d9cdd0d374fd01875379380b862a41009`  
		Last Modified: Mon, 10 May 2021 23:25:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:8917c43037c70887cbb4140acc128cea9c1c2fd7fcb70257d20145baedbd6fab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:4.4.6-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:c1c7f59a7f29591106d067877ad4e568d260572adcd9803d1fef162ca4ec9a22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:4.4.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:8027a70fbe7e47adb3b0970eacbbc1dd78cf06203cf320da5cdbc5cf71d3e01d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037334566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35400f2fef53c6fde1a596644884d280e42c2043b303fb8a64bf09ddebe3d0b5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:33:49 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:33:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:33:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:39:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:39:49 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:39:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa26c3b7dd5be40e6af6e110598ff8ade5597433a780e713fe02d41a01ff4ab`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcc96fa02f1eff07ba750778c31dbc2a2b2eb1205d0862a2ebe6b93c8f2785b`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264615459bc5dd410e8fdba7e066381e9fd687efbafbcbdc04d6a3c8f19ccb5`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93394405d931bc35ec98aec50a2d8664f5c0580f16dbae47c70dabbebf81356d`  
		Last Modified: Wed, 12 May 2021 00:59:03 GMT  
		Size: 241.5 MB (241547428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4854c02134142d249afb7fb7045fd09f266e95fce580e919b709b8dac5572bc`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea254f563aa38c2c7a29f573537255e55d3b9e8ab8c43bd857e1e8ea156bb9c4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0592557aaf1bfb0d38c61451aa21ccc7d3b5e447d85f6e38b920c27ebc0eb7b4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:3dbb3b4b8f33c8a61fa72cf1d05398d6cc09c72aa2a1f664b639d8231b0e83ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:ebb6b8403c1f47069b099f1ba75778d41e15a5d8eed3db6f435733333e403a2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175677269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07630e791de3ceb87d39543799438e118753246d19dcfd6529bd4d27ff1b83bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:58 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 00:41:59 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:11:00 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:11:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:11:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:11:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:11:48 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:11:49 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:11:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:11:49 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:11:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2ff17242ce7e307fbd191a597f210061566606443ff6632ca685d394cb9acf`  
		Last Modified: Sat, 24 Apr 2021 00:44:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11b2ce05942f19ca819aa8c130575b0850153384fba7f489fd1a62ec0d94e7`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91532386f4ec7af743bc43ddbab8410d9d2fee68ce63bca3aa397c04e29b9091`  
		Last Modified: Tue, 11 May 2021 00:12:51 GMT  
		Size: 140.2 MB (140162019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705ef0ab262e766f32008195b4e3719f5444b83e3218dbab09f5cfa7098322ea`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6238126b609f01bb47ddd8598f331bb5cb7653f2d9798eb2f14d48061d8e279`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 4.5 KB (4477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8f2c9016beb50c2972e54c732d8dc24fb332360104b9e71767af9c4e71c1348e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168070890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3a757873434f9961cb2b732f35c712866d65e5fdf009c9b8572d46c0657e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 01:53:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:53:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:08 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 01:41:03 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 01:41:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 01:41:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 01:41:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 01:41:41 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 01:41:42 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 01:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:41:44 GMT
EXPOSE 27017
# Tue, 11 May 2021 01:41:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b8f707197ef2788f2ed0cf82b088b9262efb9b7a374da64bb70daccca6525`  
		Last Modified: Sat, 24 Apr 2021 01:56:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d9f84ef7c607013458b7c4f0045d42081a3cd4e32e09a99c45af7af1742eb`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a71fa0bced6eaef2a94dfda7f28a3c97b1f52e0def1e877932edf84e97df5`  
		Last Modified: Tue, 11 May 2021 01:42:41 GMT  
		Size: 136.3 MB (136341433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88698b947abf4aa832fdbc0c629195e7b8ad1790baad6dfa6ad42b0201e5b81e`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7dfc922696b1eae0c53f3c4559bdfca5ae0dd740a6c3e5166c0839e4ce49ad`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:c8e981f281462baf0c84890eab82c4fad6c825d221664b463ccd43485f6380cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169474559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8b1f024425214a141ef62568a875dc3f443453094dbe43757c3a42d5ada69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:51:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Apr 2021 22:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:51:56 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 22:51:57 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Apr 2021 22:52:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 22:52:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 22:52:19 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 23 Apr 2021 22:52:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:24 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:38:53 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:38:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:39:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:39:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:39:55 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:39:55 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:39:56 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:39:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bc20f34c3c0e6defa11123a46488ad9866f1cbed77d74904f7b057f014902`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934bd72760b936ef87cda05b4fd31a1266859e77f6960e8b6a17eb4df55b82b2`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 2.7 MB (2708330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778576254d798d87ee503dd46947744945440e160227cf20f86506eb7f0c752`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 5.7 MB (5747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b7218def3876e2bd7ede8db669dd67c94e3f67db5c8b385e7d0b189c70f19`  
		Last Modified: Fri, 23 Apr 2021 22:53:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218c55b05ae6da8d768db66caf009228dd32c56943df536e02932cd24a359f1e`  
		Last Modified: Fri, 23 Apr 2021 22:53:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921db7ddca2b72930c0ba65cfcf991843ce2fdee70e5ed022876b6f5bebbe5`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c499f2e405c30092431c8a9e2734154a24af4ed421ff0c7d97b16d1b02f39`  
		Last Modified: Tue, 11 May 2021 00:40:40 GMT  
		Size: 135.7 MB (135656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1d700e09af9f173c1ca948355e0d1a01b5c6139b36889ca0621055669821f9`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99d8d95772dfd5147e631e7e072172ebe7c33d5d8916e8f372607a7c866572`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:401ae88210c708d54873af22df618b46a5f3d2da1c2676d115326b205ec78d3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:ebb6b8403c1f47069b099f1ba75778d41e15a5d8eed3db6f435733333e403a2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175677269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07630e791de3ceb87d39543799438e118753246d19dcfd6529bd4d27ff1b83bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:41:08 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 00:41:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:41:18 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:41:18 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 00:41:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:41:58 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 00:41:59 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 00:42:00 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 00:42:00 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:11:00 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:11:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:11:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:11:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:11:48 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:11:49 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:11:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:11:49 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:11:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d5e5c7eab9e07a520aed11bed2b4b7c44c3ec3df6e389bc458cb25c18582ad`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43798cf18b45dce7601f8c40514229531dd9f36d588b6d69b29fe7400aa80640`  
		Last Modified: Sat, 24 Apr 2021 00:43:51 GMT  
		Size: 3.0 MB (2978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67349a81f4351858274518ff0d80ad12763635a544d8483bdfc9a9d33882be7d`  
		Last Modified: Sat, 24 Apr 2021 00:43:52 GMT  
		Size: 5.8 MB (5829871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590845b1f17c5e6f8c9aef645fc7a87e9d5bf7b95a9cb3b37ccd407f7d956818`  
		Last Modified: Sat, 24 Apr 2021 00:43:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2ff17242ce7e307fbd191a597f210061566606443ff6632ca685d394cb9acf`  
		Last Modified: Sat, 24 Apr 2021 00:44:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11b2ce05942f19ca819aa8c130575b0850153384fba7f489fd1a62ec0d94e7`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91532386f4ec7af743bc43ddbab8410d9d2fee68ce63bca3aa397c04e29b9091`  
		Last Modified: Tue, 11 May 2021 00:12:51 GMT  
		Size: 140.2 MB (140162019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705ef0ab262e766f32008195b4e3719f5444b83e3218dbab09f5cfa7098322ea`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6238126b609f01bb47ddd8598f331bb5cb7653f2d9798eb2f14d48061d8e279`  
		Last Modified: Tue, 11 May 2021 00:12:27 GMT  
		Size: 4.5 KB (4477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8f2c9016beb50c2972e54c732d8dc24fb332360104b9e71767af9c4e71c1348e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168070890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3a757873434f9961cb2b732f35c712866d65e5fdf009c9b8572d46c0657e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 24 Apr 2021 01:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:51:12 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:51:13 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 24 Apr 2021 01:51:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:51:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 24 Apr 2021 01:53:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 24 Apr 2021 01:53:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 24 Apr 2021 01:53:08 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 01:41:03 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 01:41:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 01:41:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 01:41:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 01:41:41 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 01:41:42 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 01:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 01:41:44 GMT
EXPOSE 27017
# Tue, 11 May 2021 01:41:45 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd458c20dd1c19d434f0119064aff9a6faf6ac2dbdcc6cd45f6bdfbacaa0b4b`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1c02642395dddcbfb01a3b296ea1a917e26c7673a10e46ff09322af211baca`  
		Last Modified: Sat, 24 Apr 2021 01:55:38 GMT  
		Size: 2.7 MB (2669108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d074f6952b5e68616af94037f39c46fb7aa3e42a70c70538eb3a575b1c1441`  
		Last Modified: Sat, 24 Apr 2021 01:55:37 GMT  
		Size: 5.3 MB (5347272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811aaa41efc3934670804e5d37bfd7cdb0c19756c8fb60094033d31e420ebd70`  
		Last Modified: Sat, 24 Apr 2021 01:55:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b8f707197ef2788f2ed0cf82b088b9262efb9b7a374da64bb70daccca6525`  
		Last Modified: Sat, 24 Apr 2021 01:56:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d9f84ef7c607013458b7c4f0045d42081a3cd4e32e09a99c45af7af1742eb`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a71fa0bced6eaef2a94dfda7f28a3c97b1f52e0def1e877932edf84e97df5`  
		Last Modified: Tue, 11 May 2021 01:42:41 GMT  
		Size: 136.3 MB (136341433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88698b947abf4aa832fdbc0c629195e7b8ad1790baad6dfa6ad42b0201e5b81e`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7dfc922696b1eae0c53f3c4559bdfca5ae0dd740a6c3e5166c0839e4ce49ad`  
		Last Modified: Tue, 11 May 2021 01:42:14 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:c8e981f281462baf0c84890eab82c4fad6c825d221664b463ccd43485f6380cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169474559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8b1f024425214a141ef62568a875dc3f443453094dbe43757c3a42d5ada69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:00 GMT
ADD file:5e61a5300d520d61a2130623465ba2e46da8e80dc2afa042473a42cbcd8d88d2 in / 
# Fri, 23 Apr 2021 21:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:07 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:07 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:51:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Apr 2021 22:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:51:56 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 22:51:57 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Apr 2021 22:52:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 22:52:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 22:52:19 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 23 Apr 2021 22:52:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Apr 2021 22:52:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Apr 2021 22:52:24 GMT
ENV MONGO_MAJOR=4.4
# Tue, 11 May 2021 00:38:53 GMT
ENV MONGO_VERSION=4.4.6
# Tue, 11 May 2021 00:38:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 11 May 2021 00:39:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 11 May 2021 00:39:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 11 May 2021 00:39:55 GMT
VOLUME [/data/db /data/configdb]
# Tue, 11 May 2021 00:39:55 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Tue, 11 May 2021 00:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 May 2021 00:39:56 GMT
EXPOSE 27017
# Tue, 11 May 2021 00:39:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:33ddddc4572ffe1f294f9f599ed989cc41eee5da4cdcf7db12d10700aa8c894e`  
		Last Modified: Fri, 23 Apr 2021 21:47:03 GMT  
		Size: 25.4 MB (25352756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4395f372a786db91b2f50dc8e43d8b7c3533eb4bd86f6728eb2a0c7108c077d2`  
		Last Modified: Fri, 23 Apr 2021 21:46:59 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e39753730df188282ca8193f14bbbb8cbe0b76ec02b34283a28449b1e41c05`  
		Last Modified: Fri, 23 Apr 2021 21:47:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bc20f34c3c0e6defa11123a46488ad9866f1cbed77d74904f7b057f014902`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934bd72760b936ef87cda05b4fd31a1266859e77f6960e8b6a17eb4df55b82b2`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 2.7 MB (2708330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778576254d798d87ee503dd46947744945440e160227cf20f86506eb7f0c752`  
		Last Modified: Fri, 23 Apr 2021 22:53:55 GMT  
		Size: 5.7 MB (5747416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446b7218def3876e2bd7ede8db669dd67c94e3f67db5c8b385e7d0b189c70f19`  
		Last Modified: Fri, 23 Apr 2021 22:53:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218c55b05ae6da8d768db66caf009228dd32c56943df536e02932cd24a359f1e`  
		Last Modified: Fri, 23 Apr 2021 22:53:52 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921db7ddca2b72930c0ba65cfcf991843ce2fdee70e5ed022876b6f5bebbe5`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c499f2e405c30092431c8a9e2734154a24af4ed421ff0c7d97b16d1b02f39`  
		Last Modified: Tue, 11 May 2021 00:40:40 GMT  
		Size: 135.7 MB (135656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1d700e09af9f173c1ca948355e0d1a01b5c6139b36889ca0621055669821f9`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99d8d95772dfd5147e631e7e072172ebe7c33d5d8916e8f372607a7c866572`  
		Last Modified: Tue, 11 May 2021 00:40:23 GMT  
		Size: 4.5 KB (4475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:8027a70fbe7e47adb3b0970eacbbc1dd78cf06203cf320da5cdbc5cf71d3e01d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037334566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35400f2fef53c6fde1a596644884d280e42c2043b303fb8a64bf09ddebe3d0b5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:33:49 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:33:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:33:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:39:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:39:49 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:39:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa26c3b7dd5be40e6af6e110598ff8ade5597433a780e713fe02d41a01ff4ab`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcc96fa02f1eff07ba750778c31dbc2a2b2eb1205d0862a2ebe6b93c8f2785b`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264615459bc5dd410e8fdba7e066381e9fd687efbafbcbdc04d6a3c8f19ccb5`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93394405d931bc35ec98aec50a2d8664f5c0580f16dbae47c70dabbebf81356d`  
		Last Modified: Wed, 12 May 2021 00:59:03 GMT  
		Size: 241.5 MB (241547428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4854c02134142d249afb7fb7045fd09f266e95fce580e919b709b8dac5572bc`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea254f563aa38c2c7a29f573537255e55d3b9e8ab8c43bd857e1e8ea156bb9c4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0592557aaf1bfb0d38c61451aa21ccc7d3b5e447d85f6e38b920c27ebc0eb7b4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:eb0c7d46164fd225423e2c0fc64e96f52c38b738f8fd9ccba13e56c4eb119275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `mongo:windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull mongo@sha256:e2dc6e2ce10059a0d52f2e7ef003b495ed57e72c0b0e00bac2148b20dec63355
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706212737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ddc9cab99b833b8495cc7ee447d7c65463a6c877af4d80d4aa833b6d64b99a5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 10 May 2021 23:15:58 GMT
ENV MONGO_VERSION=4.4.6
# Mon, 10 May 2021 23:15:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Mon, 10 May 2021 23:16:01 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Mon, 10 May 2021 23:18:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 10 May 2021 23:18:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 10 May 2021 23:18:25 GMT
EXPOSE 27017
# Mon, 10 May 2021 23:18:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1af6a38cdaf02b9763a51588fe3ec107b6324e3c240b81be1c53374619c675`  
		Last Modified: Mon, 10 May 2021 23:24:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4550f7fa25bb90c099b1eac08fa398f54f44d40adeb082ad7c38a62223c6a411`  
		Last Modified: Mon, 10 May 2021 23:24:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfdfb1c878583e1857a026502bc1d5644702990001c8ed20f4b1b647706c59b`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417a1588a5fc27f1d60b2a2ea14002824a5de37b9d3ad7ccbb2484e44c3a9dcf`  
		Last Modified: Mon, 10 May 2021 23:24:48 GMT  
		Size: 236.4 MB (236448794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed7b32008983c9797db237aa9a90c851d502b47467b518ec9060f17065ca44`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b56283a6d31ef57873809be37e8516d0606ab794493b8237b90eb5b91be6b2`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb68b8b769ff2ae29874c729c09a2db8d3e7e0727b7b486792074d26ff7d802`  
		Last Modified: Mon, 10 May 2021 23:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull mongo@sha256:2eac7d1f71ed080a26b742240fe92543fe2e940bb5a48fdd59ac3fecc0e9e73c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6036382733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03eb8c7454248dc61a5ae434a904103696979b3e44430a44cedeb70ec3b92a7a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 10 May 2021 23:18:41 GMT
ENV MONGO_VERSION=4.4.6
# Mon, 10 May 2021 23:18:43 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Mon, 10 May 2021 23:18:44 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Mon, 10 May 2021 23:22:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 10 May 2021 23:22:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 10 May 2021 23:22:16 GMT
EXPOSE 27017
# Mon, 10 May 2021 23:22:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b78e3aa88d4e50d3d51ac081c91eeef9933d4a7a75f4845821519ed2bd1a3`  
		Last Modified: Mon, 10 May 2021 23:25:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f41596dd2dda6342571328e8de671fc73c58da781f443547f9bd94b2e602a1a`  
		Last Modified: Mon, 10 May 2021 23:25:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0fd0da468dbf2b3fb5817a9dfe9badc42a5ae933fe238ba533b51dcd548b8`  
		Last Modified: Mon, 10 May 2021 23:25:06 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228c37f48edb438de1305cde961522a16d6041442f1b377b315370fad7c041c`  
		Last Modified: Mon, 10 May 2021 23:26:04 GMT  
		Size: 241.5 MB (241488971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94206c6a1738fc370c80eb4e0259a1a74df12b0c8fa4fd45227cbd18d38bbf1`  
		Last Modified: Mon, 10 May 2021 23:25:05 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4cfcf8250b04c427f36ba05bef1ef1e42cb65e92b9f3cc2fd3f3c4fc976c65`  
		Last Modified: Mon, 10 May 2021 23:25:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0f9cb3fef403e1662a10830f0d076d9cdd0d374fd01875379380b862a41009`  
		Last Modified: Mon, 10 May 2021 23:25:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:8917c43037c70887cbb4140acc128cea9c1c2fd7fcb70257d20145baedbd6fab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:c1c7f59a7f29591106d067877ad4e568d260572adcd9803d1fef162ca4ec9a22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull mongo@sha256:8027a70fbe7e47adb3b0970eacbbc1dd78cf06203cf320da5cdbc5cf71d3e01d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037334566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35400f2fef53c6fde1a596644884d280e42c2043b303fb8a64bf09ddebe3d0b5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:33:49 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:33:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:33:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:39:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:39:49 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:39:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa26c3b7dd5be40e6af6e110598ff8ade5597433a780e713fe02d41a01ff4ab`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcc96fa02f1eff07ba750778c31dbc2a2b2eb1205d0862a2ebe6b93c8f2785b`  
		Last Modified: Wed, 12 May 2021 00:54:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264615459bc5dd410e8fdba7e066381e9fd687efbafbcbdc04d6a3c8f19ccb5`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93394405d931bc35ec98aec50a2d8664f5c0580f16dbae47c70dabbebf81356d`  
		Last Modified: Wed, 12 May 2021 00:59:03 GMT  
		Size: 241.5 MB (241547428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4854c02134142d249afb7fb7045fd09f266e95fce580e919b709b8dac5572bc`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea254f563aa38c2c7a29f573537255e55d3b9e8ab8c43bd857e1e8ea156bb9c4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0592557aaf1bfb0d38c61451aa21ccc7d3b5e447d85f6e38b920c27ebc0eb7b4`  
		Last Modified: Wed, 12 May 2021 00:54:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
