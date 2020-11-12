<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.20`](#mongo3620)
-	[`mongo:3.6.20-windowsservercore`](#mongo3620-windowsservercore)
-	[`mongo:3.6.20-windowsservercore-1809`](#mongo3620-windowsservercore-1809)
-	[`mongo:3.6.20-windowsservercore-ltsc2016`](#mongo3620-windowsservercore-ltsc2016)
-	[`mongo:3.6.20-xenial`](#mongo3620-xenial)
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
-	[`mongo:4.0.20`](#mongo4020)
-	[`mongo:4.0.20-windowsservercore`](#mongo4020-windowsservercore)
-	[`mongo:4.0.20-windowsservercore-1809`](#mongo4020-windowsservercore-1809)
-	[`mongo:4.0.20-windowsservercore-ltsc2016`](#mongo4020-windowsservercore-ltsc2016)
-	[`mongo:4.0.20-xenial`](#mongo4020-xenial)
-	[`mongo:4.0-windowsservercore`](#mongo40-windowsservercore)
-	[`mongo:4.0-windowsservercore-1809`](#mongo40-windowsservercore-1809)
-	[`mongo:4.0-windowsservercore-ltsc2016`](#mongo40-windowsservercore-ltsc2016)
-	[`mongo:4.0-xenial`](#mongo40-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2.10`](#mongo4210)
-	[`mongo:4.2.10-bionic`](#mongo4210-bionic)
-	[`mongo:4.2.10-windowsservercore`](#mongo4210-windowsservercore)
-	[`mongo:4.2.10-windowsservercore-1809`](#mongo4210-windowsservercore-1809)
-	[`mongo:4.2.10-windowsservercore-ltsc2016`](#mongo4210-windowsservercore-ltsc2016)
-	[`mongo:4.2-bionic`](#mongo42-bionic)
-	[`mongo:4.2-windowsservercore`](#mongo42-windowsservercore)
-	[`mongo:4.2-windowsservercore-1809`](#mongo42-windowsservercore-1809)
-	[`mongo:4.2-windowsservercore-ltsc2016`](#mongo42-windowsservercore-ltsc2016)
-	[`mongo:4.4`](#mongo44)
-	[`mongo:4.4.1`](#mongo441)
-	[`mongo:4.4.1-bionic`](#mongo441-bionic)
-	[`mongo:4.4.1-windowsservercore`](#mongo441-windowsservercore)
-	[`mongo:4.4.1-windowsservercore-1809`](#mongo441-windowsservercore-1809)
-	[`mongo:4.4.1-windowsservercore-ltsc2016`](#mongo441-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:0f939abf087793b53997771ea053c9a17631ff9e7bef89884e5feec1cdeb83a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:9d96d0d56a44e2e0c20dded29c6017ae878fd7a8566162e98aa770dfaecff608
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167439442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af40c6796a735b4902cab7a2004c4d3f6678f71ae5166d2233d7bb2793103cb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:18:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 23 Oct 2020 18:18:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_MAJOR=3.6
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 23 Oct 2020 18:18:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:08 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:08 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:08 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:09 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299eaf21db23f042463bcd03ff6b2e0b143d947a03c8a73ad0a600de2d2de676`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86160728082d5e4dca1dcba55260bc04b117d23240f447c5f67297b219df3478`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a4f4ac0278459f971fa1e542271449551497e63142be9a12c96c9408740e4a`  
		Last Modified: Fri, 23 Oct 2020 18:20:23 GMT  
		Size: 117.4 MB (117394719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfbc3e9d94278947db35f1072d89c68609498f69789e3fe3b16e3a1268fa3`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860826a14805c1bce5344447510517a26e19a5a6b1072fcb1dc0681e072f07f`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e12fe255885303111601cb3c605190a105eb6641ab3299b67fda4cad6b97bec3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156110815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c524e421c04d2388efa9abc4c2ba15d527de8f8db3a3457f33c291112030c2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:03 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 06 Nov 2020 04:23:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:23:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:23:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_MAJOR=3.6
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 06 Nov 2020 04:23:11 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:23:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:23:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:23:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:23:41 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:23:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:23:42 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:23:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57cb59f958e16818b7a55c704525864c33c8e1d50e46cfdfefbddde64dfe55`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823779865385a2d45416b4ca470aba36e2e8a82a0316b014ac796ace027f7997`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df99e61a8ad73557c05e77e3d5223429401ecf4a8305649c4a7852de16b1e225`  
		Last Modified: Fri, 06 Nov 2020 04:25:36 GMT  
		Size: 111.6 MB (111602560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7f192b06d6e3ba1e9eb52148c0b3da0413c05f275ce535d1e16975ed59d9a6`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86e973406889a4570586239562cdf0562f268381ce64f70b96bd4a5a692213`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:0f939abf087793b53997771ea053c9a17631ff9e7bef89884e5feec1cdeb83a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:9d96d0d56a44e2e0c20dded29c6017ae878fd7a8566162e98aa770dfaecff608
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167439442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af40c6796a735b4902cab7a2004c4d3f6678f71ae5166d2233d7bb2793103cb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:18:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 23 Oct 2020 18:18:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_MAJOR=3.6
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 23 Oct 2020 18:18:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:08 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:08 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:08 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:09 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299eaf21db23f042463bcd03ff6b2e0b143d947a03c8a73ad0a600de2d2de676`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86160728082d5e4dca1dcba55260bc04b117d23240f447c5f67297b219df3478`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a4f4ac0278459f971fa1e542271449551497e63142be9a12c96c9408740e4a`  
		Last Modified: Fri, 23 Oct 2020 18:20:23 GMT  
		Size: 117.4 MB (117394719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfbc3e9d94278947db35f1072d89c68609498f69789e3fe3b16e3a1268fa3`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860826a14805c1bce5344447510517a26e19a5a6b1072fcb1dc0681e072f07f`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e12fe255885303111601cb3c605190a105eb6641ab3299b67fda4cad6b97bec3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156110815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c524e421c04d2388efa9abc4c2ba15d527de8f8db3a3457f33c291112030c2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:03 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 06 Nov 2020 04:23:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:23:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:23:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_MAJOR=3.6
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 06 Nov 2020 04:23:11 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:23:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:23:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:23:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:23:41 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:23:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:23:42 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:23:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57cb59f958e16818b7a55c704525864c33c8e1d50e46cfdfefbddde64dfe55`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823779865385a2d45416b4ca470aba36e2e8a82a0316b014ac796ace027f7997`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df99e61a8ad73557c05e77e3d5223429401ecf4a8305649c4a7852de16b1e225`  
		Last Modified: Fri, 06 Nov 2020 04:25:36 GMT  
		Size: 111.6 MB (111602560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7f192b06d6e3ba1e9eb52148c0b3da0413c05f275ce535d1e16975ed59d9a6`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86e973406889a4570586239562cdf0562f268381ce64f70b96bd4a5a692213`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.20`

```console
$ docker pull mongo@sha256:0f939abf087793b53997771ea053c9a17631ff9e7bef89884e5feec1cdeb83a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:3.6.20` - linux; amd64

```console
$ docker pull mongo@sha256:9d96d0d56a44e2e0c20dded29c6017ae878fd7a8566162e98aa770dfaecff608
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167439442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af40c6796a735b4902cab7a2004c4d3f6678f71ae5166d2233d7bb2793103cb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:18:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 23 Oct 2020 18:18:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_MAJOR=3.6
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 23 Oct 2020 18:18:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:08 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:08 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:08 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:09 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299eaf21db23f042463bcd03ff6b2e0b143d947a03c8a73ad0a600de2d2de676`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86160728082d5e4dca1dcba55260bc04b117d23240f447c5f67297b219df3478`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a4f4ac0278459f971fa1e542271449551497e63142be9a12c96c9408740e4a`  
		Last Modified: Fri, 23 Oct 2020 18:20:23 GMT  
		Size: 117.4 MB (117394719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfbc3e9d94278947db35f1072d89c68609498f69789e3fe3b16e3a1268fa3`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860826a14805c1bce5344447510517a26e19a5a6b1072fcb1dc0681e072f07f`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.20` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e12fe255885303111601cb3c605190a105eb6641ab3299b67fda4cad6b97bec3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156110815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c524e421c04d2388efa9abc4c2ba15d527de8f8db3a3457f33c291112030c2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:03 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 06 Nov 2020 04:23:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:23:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:23:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_MAJOR=3.6
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 06 Nov 2020 04:23:11 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:23:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:23:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:23:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:23:41 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:23:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:23:42 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:23:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57cb59f958e16818b7a55c704525864c33c8e1d50e46cfdfefbddde64dfe55`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823779865385a2d45416b4ca470aba36e2e8a82a0316b014ac796ace027f7997`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df99e61a8ad73557c05e77e3d5223429401ecf4a8305649c4a7852de16b1e225`  
		Last Modified: Fri, 06 Nov 2020 04:25:36 GMT  
		Size: 111.6 MB (111602560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7f192b06d6e3ba1e9eb52148c0b3da0413c05f275ce535d1e16975ed59d9a6`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86e973406889a4570586239562cdf0562f268381ce64f70b96bd4a5a692213`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.20` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.20` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.20-windowsservercore`

```console
$ docker pull mongo@sha256:6744de11f9597269b0b1eb8a2a2f82dfd4fac2859da021a31bb0090ab9efb5f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:3.6.20-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.20-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.20-windowsservercore-1809`

```console
$ docker pull mongo@sha256:7d3b86ea295599fd398a6ce78039a210b3c6e1fb4e9dff7e1ef71ddaaa5c9a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:3.6.20-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.20-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:34342e4f7e97658b03d1481ff362b12cff15d4a0e446b59bbc126b7a76bd45ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:3.6.20-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.20-xenial`

```console
$ docker pull mongo@sha256:59dd2907c80214dade6b50f5077fa4708dd9818d115ba0a7a1595bed6657383f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.20-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:9d96d0d56a44e2e0c20dded29c6017ae878fd7a8566162e98aa770dfaecff608
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167439442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af40c6796a735b4902cab7a2004c4d3f6678f71ae5166d2233d7bb2793103cb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:18:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 23 Oct 2020 18:18:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_MAJOR=3.6
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 23 Oct 2020 18:18:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:08 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:08 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:08 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:09 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299eaf21db23f042463bcd03ff6b2e0b143d947a03c8a73ad0a600de2d2de676`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86160728082d5e4dca1dcba55260bc04b117d23240f447c5f67297b219df3478`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a4f4ac0278459f971fa1e542271449551497e63142be9a12c96c9408740e4a`  
		Last Modified: Fri, 23 Oct 2020 18:20:23 GMT  
		Size: 117.4 MB (117394719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfbc3e9d94278947db35f1072d89c68609498f69789e3fe3b16e3a1268fa3`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860826a14805c1bce5344447510517a26e19a5a6b1072fcb1dc0681e072f07f`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.20-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e12fe255885303111601cb3c605190a105eb6641ab3299b67fda4cad6b97bec3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156110815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c524e421c04d2388efa9abc4c2ba15d527de8f8db3a3457f33c291112030c2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:03 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 06 Nov 2020 04:23:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:23:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:23:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_MAJOR=3.6
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 06 Nov 2020 04:23:11 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:23:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:23:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:23:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:23:41 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:23:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:23:42 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:23:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57cb59f958e16818b7a55c704525864c33c8e1d50e46cfdfefbddde64dfe55`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823779865385a2d45416b4ca470aba36e2e8a82a0316b014ac796ace027f7997`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df99e61a8ad73557c05e77e3d5223429401ecf4a8305649c4a7852de16b1e225`  
		Last Modified: Fri, 06 Nov 2020 04:25:36 GMT  
		Size: 111.6 MB (111602560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7f192b06d6e3ba1e9eb52148c0b3da0413c05f275ce535d1e16975ed59d9a6`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86e973406889a4570586239562cdf0562f268381ce64f70b96bd4a5a692213`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:6744de11f9597269b0b1eb8a2a2f82dfd4fac2859da021a31bb0090ab9efb5f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:7d3b86ea295599fd398a6ce78039a210b3c6e1fb4e9dff7e1ef71ddaaa5c9a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:34342e4f7e97658b03d1481ff362b12cff15d4a0e446b59bbc126b7a76bd45ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:59dd2907c80214dade6b50f5077fa4708dd9818d115ba0a7a1595bed6657383f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:9d96d0d56a44e2e0c20dded29c6017ae878fd7a8566162e98aa770dfaecff608
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167439442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af40c6796a735b4902cab7a2004c4d3f6678f71ae5166d2233d7bb2793103cb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:18:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 23 Oct 2020 18:18:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_MAJOR=3.6
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 23 Oct 2020 18:18:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:08 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:08 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:08 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:09 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299eaf21db23f042463bcd03ff6b2e0b143d947a03c8a73ad0a600de2d2de676`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86160728082d5e4dca1dcba55260bc04b117d23240f447c5f67297b219df3478`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a4f4ac0278459f971fa1e542271449551497e63142be9a12c96c9408740e4a`  
		Last Modified: Fri, 23 Oct 2020 18:20:23 GMT  
		Size: 117.4 MB (117394719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfbc3e9d94278947db35f1072d89c68609498f69789e3fe3b16e3a1268fa3`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860826a14805c1bce5344447510517a26e19a5a6b1072fcb1dc0681e072f07f`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e12fe255885303111601cb3c605190a105eb6641ab3299b67fda4cad6b97bec3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156110815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c524e421c04d2388efa9abc4c2ba15d527de8f8db3a3457f33c291112030c2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:03 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 06 Nov 2020 04:23:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:23:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:23:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_MAJOR=3.6
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 06 Nov 2020 04:23:11 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:23:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:23:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:23:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:23:41 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:23:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:23:42 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:23:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57cb59f958e16818b7a55c704525864c33c8e1d50e46cfdfefbddde64dfe55`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823779865385a2d45416b4ca470aba36e2e8a82a0316b014ac796ace027f7997`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df99e61a8ad73557c05e77e3d5223429401ecf4a8305649c4a7852de16b1e225`  
		Last Modified: Fri, 06 Nov 2020 04:25:36 GMT  
		Size: 111.6 MB (111602560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7f192b06d6e3ba1e9eb52148c0b3da0413c05f275ce535d1e16975ed59d9a6`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86e973406889a4570586239562cdf0562f268381ce64f70b96bd4a5a692213`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:6744de11f9597269b0b1eb8a2a2f82dfd4fac2859da021a31bb0090ab9efb5f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:3-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:7d3b86ea295599fd398a6ce78039a210b3c6e1fb4e9dff7e1ef71ddaaa5c9a83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:59b45e44959ed05701050353c8f75909126b4753934a8b35b90c7e7312540934
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2618107146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1f6f335c1565f62b16b3279025d447d7eea2ede1cf1091dcadeefce882319`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:35:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:36:00 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:55:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:55:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:55:33 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:55:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d809ace595405ac85dfb43a590428989c3ed42c4d21311f29e0a8aeea1c477a`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd674f51d7fb6787d9d0e51cadd38969f4d4564c9f42b845b0e6ce777f8b31cc`  
		Last Modified: Wed, 11 Nov 2020 23:56:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cdb7bcfe48bcb690c0aaec1bdfc86ccabd64940d6185c8d6bd8f1f52ee5c8`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceed10ea0daa314db1e6fec268390a7be6cc1598d8eb472bceaa36bc2ec5b03`  
		Last Modified: Wed, 11 Nov 2020 23:57:10 GMT  
		Size: 230.1 MB (230069869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c31d44a13eae8ee31b6eec4b26329bba8735405422b60a0d6e4b4b1688636`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786221bc9bc9f05d378b09a28ef9ab168e6099a555112b9174e50640d5e94479`  
		Last Modified: Wed, 11 Nov 2020 23:56:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c97c634a8c5a73a0e0fc4f0b0f4018cf24351583f51b5cab677a5e975a91a4`  
		Last Modified: Wed, 11 Nov 2020 23:56:24 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:34342e4f7e97658b03d1481ff362b12cff15d4a0e446b59bbc126b7a76bd45ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:59dd2907c80214dade6b50f5077fa4708dd9818d115ba0a7a1595bed6657383f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:9d96d0d56a44e2e0c20dded29c6017ae878fd7a8566162e98aa770dfaecff608
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167439442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af40c6796a735b4902cab7a2004c4d3f6678f71ae5166d2233d7bb2793103cb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:18:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 23 Oct 2020 18:18:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:18:48 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_MAJOR=3.6
# Fri, 23 Oct 2020 18:18:48 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 23 Oct 2020 18:18:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:08 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:08 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:08 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:09 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299eaf21db23f042463bcd03ff6b2e0b143d947a03c8a73ad0a600de2d2de676`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86160728082d5e4dca1dcba55260bc04b117d23240f447c5f67297b219df3478`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a4f4ac0278459f971fa1e542271449551497e63142be9a12c96c9408740e4a`  
		Last Modified: Fri, 23 Oct 2020 18:20:23 GMT  
		Size: 117.4 MB (117394719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfbc3e9d94278947db35f1072d89c68609498f69789e3fe3b16e3a1268fa3`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860826a14805c1bce5344447510517a26e19a5a6b1072fcb1dc0681e072f07f`  
		Last Modified: Fri, 23 Oct 2020 18:20:05 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e12fe255885303111601cb3c605190a105eb6641ab3299b67fda4cad6b97bec3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156110815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c524e421c04d2388efa9abc4c2ba15d527de8f8db3a3457f33c291112030c2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:03 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 06 Nov 2020 04:23:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:23:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:23:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_MAJOR=3.6
# Fri, 06 Nov 2020 04:23:09 GMT
ENV MONGO_VERSION=3.6.20
# Fri, 06 Nov 2020 04:23:11 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:23:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:23:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:23:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:23:41 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:23:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:23:42 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:23:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57cb59f958e16818b7a55c704525864c33c8e1d50e46cfdfefbddde64dfe55`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823779865385a2d45416b4ca470aba36e2e8a82a0316b014ac796ace027f7997`  
		Last Modified: Fri, 06 Nov 2020 04:25:12 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df99e61a8ad73557c05e77e3d5223429401ecf4a8305649c4a7852de16b1e225`  
		Last Modified: Fri, 06 Nov 2020 04:25:36 GMT  
		Size: 111.6 MB (111602560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7f192b06d6e3ba1e9eb52148c0b3da0413c05f275ce535d1e16975ed59d9a6`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86e973406889a4570586239562cdf0562f268381ce64f70b96bd4a5a692213`  
		Last Modified: Fri, 06 Nov 2020 04:25:11 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:ca31e7cf0ba12b6e7cdbf8b888a6c66f2a4351ad862e13390c9aa9e289d46701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:31f6433f7cfcd2180483e40728cbf97142df1e85de36d80d75c93e5e7fe10405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177990635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0c2ff8d3620c0910832424efef02787214013b1c5b1d9dc9d87d638e2ceb71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:52 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 26 Sep 2020 01:03:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_MAJOR=4.4
# Sat, 26 Sep 2020 01:03:54 GMT
ENV MONGO_VERSION=4.4.1
# Sat, 26 Sep 2020 01:03:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 26 Sep 2020 01:04:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 26 Sep 2020 01:04:17 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 26 Sep 2020 01:04:17 GMT
VOLUME [/data/db /data/configdb]
# Sat, 26 Sep 2020 01:04:17 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 26 Sep 2020 01:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 01:04:17 GMT
EXPOSE 27017
# Sat, 26 Sep 2020 01:04:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8e9d469d838ebf98e71cb6b3b7f8e240f3211ff9a748c2dbff89e89a6fbeb`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69705b632494baffeba7f6c1c0a94fd5ee03db85c89dfa2eaac1c63b688f0430`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7daea26376d3196b89343320721e500e9391aef836c98a11e405734c38efc03`  
		Last Modified: Sat, 26 Sep 2020 01:06:21 GMT  
		Size: 142.5 MB (142478251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1f9e1fc7786860f32896276f7d77d09229f899e165348849e9916f6a60359`  
		Last Modified: Sat, 26 Sep 2020 01:06:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e65fe7ffd2b7653fff155ba55cbb8ae920f294f1b861a71758f176cf9eaa6`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:813ecaa78bf36de902579105aac27356b2a0bd876dcc6d7fdc977cf3898191e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167940515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811d532cf7eeb16c636343bc3e183c1db7fe8d887762b141e975f74e81481e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:22:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:22:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:22:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:22:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:22:36 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:22:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:23:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:23:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:23:12 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:23:13 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:23:14 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:23:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aec146ec81548df08b7b730fc041116e64f844464070486ee95f93a41de1f3`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215b86ffc2f95704af100aec2bfabdcb5745cc2339c548fee0353eafe414f9b`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11b0a6ff5a4354355c3588f66dcfb3b8716e4fe55dda70431b330cf7756b650`  
		Last Modified: Fri, 25 Sep 2020 23:25:58 GMT  
		Size: 136.2 MB (136196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f36a0aa04da4aa9dbc7ee2f91f1c1dbc63dad241d94dc7f0c13f54734627e4`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855fdd1e2165c9684a4cf42a775a55e4a0b49138a52fbd97c97fcb547fe773c`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 3.9 KB (3948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:de1f653589e4153f89f7d242f907c69c16ea91f95f2a94240a19634aa8d57c4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172881569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc0c05512382652300ed10d809912071b8ee0ca14c10891cabccd8228c6dc94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:28:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:28:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:28:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:29:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:29:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:29:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:29:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:29:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:30:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:30:03 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:30:03 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:04 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:30:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288641caad70cb1c99ea2cd010ce53478a4fcde867a83434c8f98575f1fc90`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb83c3ffb783f1412239a892171b331eef5d68b65aae1a2c51c44619cacb1c0`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 2.7 MB (2704583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67c01a91968aa16935794fc7d52f7742b3359858bcfa36f033e3a9a8247e780`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 5.7 MB (5746126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf72d8578ae0c25477822fd40465d9f9f696e8178817341284280781fe545f9d`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f80311986b5ccb82ae38f1f7b88c67e49b6fc81534ef8984e5b2109064d6b`  
		Last Modified: Fri, 25 Sep 2020 23:30:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862844c0ef43cc7917b410c17cbcd9e60c83231627cae7f40aa92a521f4efb6`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ef58863de1fef5f933f4f05dd35e6f38ea3d1f491e4363a67c0b07db5afaa`  
		Last Modified: Fri, 25 Sep 2020 23:30:54 GMT  
		Size: 139.1 MB (139050035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36be598b0fb9cf5388c223afc27633dc987a84af1aa05cf185133ea8ce300bb8`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd583fd9ef05f53886b3c68b812186511fcd3b1ad1bcc98ca3f244eec4dc2e5`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:0e071a7c38792f428cf602b6843fb6ccfea3418e11549e13499274bc2167b78e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:74ae7e6bc9b39cc7e165f94b25b578be68a08d27ca9b1410de04ba74c9208b55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155307089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6fa3383f923c63fbffcaaf617f6f9d1b1a99b8f7fc2d3a5d8e25660e82b6e05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:19:18 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 23 Oct 2020 18:19:18 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:19:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:19:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_MAJOR=4.0
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_VERSION=4.0.20
# Fri, 23 Oct 2020 18:19:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:41 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec910c91aca5d2a75b18c619421617ea9c7cefe356af64c77910c9ac0a43bf4`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9634ed1120c7427dc3759b0230a7fe9a5b68f948358a96953096df9d755395`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff92f0f12004cf265a929ce95459961d996cb583a835a6079e4eba75268eeb9`  
		Last Modified: Fri, 23 Oct 2020 18:20:45 GMT  
		Size: 105.3 MB (105262932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d45b107e15920f784057db5618b6be3631a7386ea89804ee4c76436dd1ff8b`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6695f173ad69f19dc1befcb49fd07f0afc1b5d38513ae91f4c4ac76cb1731754`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:51b630ba0998bce10ff0d6427cc86863e7ba156e4aa02e95486a6323c217c765
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144197957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:824f07817668b9db05e258a08e96ca7d3c775514d2771f28a6447e13d0a4862f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:58 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 06 Nov 2020 04:24:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:24:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:24:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:24:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:24:04 GMT
ENV MONGO_MAJOR=4.0
# Fri, 06 Nov 2020 04:24:05 GMT
ENV MONGO_VERSION=4.0.20
# Fri, 06 Nov 2020 04:24:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:24:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:24:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:24:34 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:24:34 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:24:36 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:24:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a77d01a1b6e755afe6af91147d79c598f2ea7675b0c980e9490d298f853456`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2afa7111cdba2f4f7f4ce4ebce980756130241521a08a476b530d98951ef308`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2634e8ad74244d37ad47c2bc08072d3066d27b2bac633095126788621708b60d`  
		Last Modified: Fri, 06 Nov 2020 04:26:11 GMT  
		Size: 99.7 MB (99690270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae008ad37b51a3ff368222010a631a38d404723612c50e57a8abee888c99c4fe`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4293638312648ce4de297aa9d451ecd95bd89a915c77ff7f0091bbc728a3a2e`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:e7889807b129cfaf8285e77b9d68e4628385dd168f1172512bb2d138a2aa5519
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004538921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c1e3f5b37cccdfd64d877da154a583ff28506ccd6786e064413ebd95dc3741`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:55:47 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:00:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:00:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:00:36 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:00:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3403a8ab1a2424bec19f328e0c8db0f1b90652b0acd9a1ceb56249408b3360`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1df638978971ee88015ef27b2f87a7b7094581aee1cb17352555137d588205f`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05cd9e2eddcc06ff31a4ba6144fbe9b4eb2346d4534c55d57ac51b4e6ecb39a`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4921d494bc15f503d642ab7d7bd1951410391f505ac5ac7239a9f42c199df47a`  
		Last Modified: Wed, 11 Nov 2020 23:58:13 GMT  
		Size: 234.0 MB (233972169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafd33cde1da5d5d72101e7ea30f212e37c77400cd9baa0b6d0229a9ca39617`  
		Last Modified: Wed, 11 Nov 2020 23:57:26 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87747aed14209c176447112dc7760d74d4e433819ab80e57aa039536971a9a0`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dc1fbd73a047d45fdc7889b14d4d86e28944c52f76ffd74ccd0751667d0e46`  
		Last Modified: Wed, 11 Nov 2020 23:57:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:85c7da4f622f4905caf91ed9735baeeb94ff81b599276f8bf8f3fb0d60769baf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2620971455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e974ed52b4f6442ad7c96016e2150599c4edddc4e1a87680448e84e6605e0b3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:00:44 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 22:00:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 22:00:46 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:04:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:04:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:04:44 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:04:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95826f34968840372cf7395fcfeb007c4e01790028cbf66abf9b71b1432c789f`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc337e144872087cec71f834b17427501f8ad018507f711542e59af8b4b4df5`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde282dc14f2040cce3455570b4a87db9206c4a9a86bffd5d4d9877702dac85`  
		Last Modified: Wed, 11 Nov 2020 23:58:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c126dd795a4db16a12293c1fe16e2d83a756751ede3f642912247cf604ce0590`  
		Last Modified: Wed, 11 Nov 2020 23:59:12 GMT  
		Size: 232.9 MB (232934220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334a0c987646cd690541030ac04aaac9110da344b8306b0eab1a942c39e31fc2`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04587b3ede5db86dd3ebc5b15d785a4dde8df15fe927369d7d03cf487cc8d2a6`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abffb6c89c52efc79520d15108209c678abdebd595d86168e105f06d718ca1`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.20`

```console
$ docker pull mongo@sha256:0e071a7c38792f428cf602b6843fb6ccfea3418e11549e13499274bc2167b78e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.0.20` - linux; amd64

```console
$ docker pull mongo@sha256:74ae7e6bc9b39cc7e165f94b25b578be68a08d27ca9b1410de04ba74c9208b55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155307089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6fa3383f923c63fbffcaaf617f6f9d1b1a99b8f7fc2d3a5d8e25660e82b6e05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:19:18 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 23 Oct 2020 18:19:18 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:19:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:19:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_MAJOR=4.0
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_VERSION=4.0.20
# Fri, 23 Oct 2020 18:19:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:41 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec910c91aca5d2a75b18c619421617ea9c7cefe356af64c77910c9ac0a43bf4`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9634ed1120c7427dc3759b0230a7fe9a5b68f948358a96953096df9d755395`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff92f0f12004cf265a929ce95459961d996cb583a835a6079e4eba75268eeb9`  
		Last Modified: Fri, 23 Oct 2020 18:20:45 GMT  
		Size: 105.3 MB (105262932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d45b107e15920f784057db5618b6be3631a7386ea89804ee4c76436dd1ff8b`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6695f173ad69f19dc1befcb49fd07f0afc1b5d38513ae91f4c4ac76cb1731754`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.20` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:51b630ba0998bce10ff0d6427cc86863e7ba156e4aa02e95486a6323c217c765
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144197957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:824f07817668b9db05e258a08e96ca7d3c775514d2771f28a6447e13d0a4862f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:58 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 06 Nov 2020 04:24:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:24:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:24:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:24:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:24:04 GMT
ENV MONGO_MAJOR=4.0
# Fri, 06 Nov 2020 04:24:05 GMT
ENV MONGO_VERSION=4.0.20
# Fri, 06 Nov 2020 04:24:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:24:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:24:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:24:34 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:24:34 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:24:36 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:24:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a77d01a1b6e755afe6af91147d79c598f2ea7675b0c980e9490d298f853456`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2afa7111cdba2f4f7f4ce4ebce980756130241521a08a476b530d98951ef308`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2634e8ad74244d37ad47c2bc08072d3066d27b2bac633095126788621708b60d`  
		Last Modified: Fri, 06 Nov 2020 04:26:11 GMT  
		Size: 99.7 MB (99690270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae008ad37b51a3ff368222010a631a38d404723612c50e57a8abee888c99c4fe`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4293638312648ce4de297aa9d451ecd95bd89a915c77ff7f0091bbc728a3a2e`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.20` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:e7889807b129cfaf8285e77b9d68e4628385dd168f1172512bb2d138a2aa5519
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004538921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c1e3f5b37cccdfd64d877da154a583ff28506ccd6786e064413ebd95dc3741`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:55:47 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:00:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:00:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:00:36 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:00:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3403a8ab1a2424bec19f328e0c8db0f1b90652b0acd9a1ceb56249408b3360`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1df638978971ee88015ef27b2f87a7b7094581aee1cb17352555137d588205f`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05cd9e2eddcc06ff31a4ba6144fbe9b4eb2346d4534c55d57ac51b4e6ecb39a`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4921d494bc15f503d642ab7d7bd1951410391f505ac5ac7239a9f42c199df47a`  
		Last Modified: Wed, 11 Nov 2020 23:58:13 GMT  
		Size: 234.0 MB (233972169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafd33cde1da5d5d72101e7ea30f212e37c77400cd9baa0b6d0229a9ca39617`  
		Last Modified: Wed, 11 Nov 2020 23:57:26 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87747aed14209c176447112dc7760d74d4e433819ab80e57aa039536971a9a0`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dc1fbd73a047d45fdc7889b14d4d86e28944c52f76ffd74ccd0751667d0e46`  
		Last Modified: Wed, 11 Nov 2020 23:57:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.20` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:85c7da4f622f4905caf91ed9735baeeb94ff81b599276f8bf8f3fb0d60769baf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2620971455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e974ed52b4f6442ad7c96016e2150599c4edddc4e1a87680448e84e6605e0b3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:00:44 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 22:00:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 22:00:46 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:04:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:04:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:04:44 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:04:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95826f34968840372cf7395fcfeb007c4e01790028cbf66abf9b71b1432c789f`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc337e144872087cec71f834b17427501f8ad018507f711542e59af8b4b4df5`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde282dc14f2040cce3455570b4a87db9206c4a9a86bffd5d4d9877702dac85`  
		Last Modified: Wed, 11 Nov 2020 23:58:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c126dd795a4db16a12293c1fe16e2d83a756751ede3f642912247cf604ce0590`  
		Last Modified: Wed, 11 Nov 2020 23:59:12 GMT  
		Size: 232.9 MB (232934220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334a0c987646cd690541030ac04aaac9110da344b8306b0eab1a942c39e31fc2`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04587b3ede5db86dd3ebc5b15d785a4dde8df15fe927369d7d03cf487cc8d2a6`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abffb6c89c52efc79520d15108209c678abdebd595d86168e105f06d718ca1`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.20-windowsservercore`

```console
$ docker pull mongo@sha256:378aa5d368080e73a6923745669068cb01f771699569da7f996971432cc89e1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.0.20-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:e7889807b129cfaf8285e77b9d68e4628385dd168f1172512bb2d138a2aa5519
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004538921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c1e3f5b37cccdfd64d877da154a583ff28506ccd6786e064413ebd95dc3741`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:55:47 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:00:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:00:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:00:36 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:00:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3403a8ab1a2424bec19f328e0c8db0f1b90652b0acd9a1ceb56249408b3360`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1df638978971ee88015ef27b2f87a7b7094581aee1cb17352555137d588205f`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05cd9e2eddcc06ff31a4ba6144fbe9b4eb2346d4534c55d57ac51b4e6ecb39a`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4921d494bc15f503d642ab7d7bd1951410391f505ac5ac7239a9f42c199df47a`  
		Last Modified: Wed, 11 Nov 2020 23:58:13 GMT  
		Size: 234.0 MB (233972169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafd33cde1da5d5d72101e7ea30f212e37c77400cd9baa0b6d0229a9ca39617`  
		Last Modified: Wed, 11 Nov 2020 23:57:26 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87747aed14209c176447112dc7760d74d4e433819ab80e57aa039536971a9a0`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dc1fbd73a047d45fdc7889b14d4d86e28944c52f76ffd74ccd0751667d0e46`  
		Last Modified: Wed, 11 Nov 2020 23:57:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.20-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:85c7da4f622f4905caf91ed9735baeeb94ff81b599276f8bf8f3fb0d60769baf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2620971455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e974ed52b4f6442ad7c96016e2150599c4edddc4e1a87680448e84e6605e0b3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:00:44 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 22:00:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 22:00:46 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:04:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:04:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:04:44 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:04:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95826f34968840372cf7395fcfeb007c4e01790028cbf66abf9b71b1432c789f`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc337e144872087cec71f834b17427501f8ad018507f711542e59af8b4b4df5`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde282dc14f2040cce3455570b4a87db9206c4a9a86bffd5d4d9877702dac85`  
		Last Modified: Wed, 11 Nov 2020 23:58:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c126dd795a4db16a12293c1fe16e2d83a756751ede3f642912247cf604ce0590`  
		Last Modified: Wed, 11 Nov 2020 23:59:12 GMT  
		Size: 232.9 MB (232934220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334a0c987646cd690541030ac04aaac9110da344b8306b0eab1a942c39e31fc2`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04587b3ede5db86dd3ebc5b15d785a4dde8df15fe927369d7d03cf487cc8d2a6`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abffb6c89c52efc79520d15108209c678abdebd595d86168e105f06d718ca1`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.20-windowsservercore-1809`

```console
$ docker pull mongo@sha256:35b4c4f8ed0462222de9be676ceeb5a04cdb8db5806862949eb86b3a0caa0a48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.0.20-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:85c7da4f622f4905caf91ed9735baeeb94ff81b599276f8bf8f3fb0d60769baf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2620971455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e974ed52b4f6442ad7c96016e2150599c4edddc4e1a87680448e84e6605e0b3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:00:44 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 22:00:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 22:00:46 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:04:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:04:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:04:44 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:04:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95826f34968840372cf7395fcfeb007c4e01790028cbf66abf9b71b1432c789f`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc337e144872087cec71f834b17427501f8ad018507f711542e59af8b4b4df5`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde282dc14f2040cce3455570b4a87db9206c4a9a86bffd5d4d9877702dac85`  
		Last Modified: Wed, 11 Nov 2020 23:58:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c126dd795a4db16a12293c1fe16e2d83a756751ede3f642912247cf604ce0590`  
		Last Modified: Wed, 11 Nov 2020 23:59:12 GMT  
		Size: 232.9 MB (232934220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334a0c987646cd690541030ac04aaac9110da344b8306b0eab1a942c39e31fc2`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04587b3ede5db86dd3ebc5b15d785a4dde8df15fe927369d7d03cf487cc8d2a6`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abffb6c89c52efc79520d15108209c678abdebd595d86168e105f06d718ca1`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.20-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0c53d3180b47bbb7e6dcf3730be4fc34620ddf32b759b6d4577273c7766ad565
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:4.0.20-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:e7889807b129cfaf8285e77b9d68e4628385dd168f1172512bb2d138a2aa5519
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004538921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c1e3f5b37cccdfd64d877da154a583ff28506ccd6786e064413ebd95dc3741`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:55:47 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:00:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:00:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:00:36 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:00:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3403a8ab1a2424bec19f328e0c8db0f1b90652b0acd9a1ceb56249408b3360`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1df638978971ee88015ef27b2f87a7b7094581aee1cb17352555137d588205f`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05cd9e2eddcc06ff31a4ba6144fbe9b4eb2346d4534c55d57ac51b4e6ecb39a`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4921d494bc15f503d642ab7d7bd1951410391f505ac5ac7239a9f42c199df47a`  
		Last Modified: Wed, 11 Nov 2020 23:58:13 GMT  
		Size: 234.0 MB (233972169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafd33cde1da5d5d72101e7ea30f212e37c77400cd9baa0b6d0229a9ca39617`  
		Last Modified: Wed, 11 Nov 2020 23:57:26 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87747aed14209c176447112dc7760d74d4e433819ab80e57aa039536971a9a0`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dc1fbd73a047d45fdc7889b14d4d86e28944c52f76ffd74ccd0751667d0e46`  
		Last Modified: Wed, 11 Nov 2020 23:57:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.20-xenial`

```console
$ docker pull mongo@sha256:c206c0fed83fbb255dfe1fac6da6512b4dbbf6d217809e4b01245657bdb2995a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.20-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:74ae7e6bc9b39cc7e165f94b25b578be68a08d27ca9b1410de04ba74c9208b55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155307089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6fa3383f923c63fbffcaaf617f6f9d1b1a99b8f7fc2d3a5d8e25660e82b6e05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:19:18 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 23 Oct 2020 18:19:18 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:19:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:19:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_MAJOR=4.0
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_VERSION=4.0.20
# Fri, 23 Oct 2020 18:19:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:41 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec910c91aca5d2a75b18c619421617ea9c7cefe356af64c77910c9ac0a43bf4`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9634ed1120c7427dc3759b0230a7fe9a5b68f948358a96953096df9d755395`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff92f0f12004cf265a929ce95459961d996cb583a835a6079e4eba75268eeb9`  
		Last Modified: Fri, 23 Oct 2020 18:20:45 GMT  
		Size: 105.3 MB (105262932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d45b107e15920f784057db5618b6be3631a7386ea89804ee4c76436dd1ff8b`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6695f173ad69f19dc1befcb49fd07f0afc1b5d38513ae91f4c4ac76cb1731754`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.20-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:51b630ba0998bce10ff0d6427cc86863e7ba156e4aa02e95486a6323c217c765
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144197957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:824f07817668b9db05e258a08e96ca7d3c775514d2771f28a6447e13d0a4862f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:58 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 06 Nov 2020 04:24:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:24:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:24:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:24:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:24:04 GMT
ENV MONGO_MAJOR=4.0
# Fri, 06 Nov 2020 04:24:05 GMT
ENV MONGO_VERSION=4.0.20
# Fri, 06 Nov 2020 04:24:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:24:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:24:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:24:34 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:24:34 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:24:36 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:24:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a77d01a1b6e755afe6af91147d79c598f2ea7675b0c980e9490d298f853456`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2afa7111cdba2f4f7f4ce4ebce980756130241521a08a476b530d98951ef308`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2634e8ad74244d37ad47c2bc08072d3066d27b2bac633095126788621708b60d`  
		Last Modified: Fri, 06 Nov 2020 04:26:11 GMT  
		Size: 99.7 MB (99690270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae008ad37b51a3ff368222010a631a38d404723612c50e57a8abee888c99c4fe`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4293638312648ce4de297aa9d451ecd95bd89a915c77ff7f0091bbc728a3a2e`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:378aa5d368080e73a6923745669068cb01f771699569da7f996971432cc89e1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:e7889807b129cfaf8285e77b9d68e4628385dd168f1172512bb2d138a2aa5519
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004538921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c1e3f5b37cccdfd64d877da154a583ff28506ccd6786e064413ebd95dc3741`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:55:47 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:00:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:00:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:00:36 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:00:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3403a8ab1a2424bec19f328e0c8db0f1b90652b0acd9a1ceb56249408b3360`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1df638978971ee88015ef27b2f87a7b7094581aee1cb17352555137d588205f`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05cd9e2eddcc06ff31a4ba6144fbe9b4eb2346d4534c55d57ac51b4e6ecb39a`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4921d494bc15f503d642ab7d7bd1951410391f505ac5ac7239a9f42c199df47a`  
		Last Modified: Wed, 11 Nov 2020 23:58:13 GMT  
		Size: 234.0 MB (233972169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafd33cde1da5d5d72101e7ea30f212e37c77400cd9baa0b6d0229a9ca39617`  
		Last Modified: Wed, 11 Nov 2020 23:57:26 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87747aed14209c176447112dc7760d74d4e433819ab80e57aa039536971a9a0`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dc1fbd73a047d45fdc7889b14d4d86e28944c52f76ffd74ccd0751667d0e46`  
		Last Modified: Wed, 11 Nov 2020 23:57:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:85c7da4f622f4905caf91ed9735baeeb94ff81b599276f8bf8f3fb0d60769baf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2620971455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e974ed52b4f6442ad7c96016e2150599c4edddc4e1a87680448e84e6605e0b3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:00:44 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 22:00:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 22:00:46 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:04:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:04:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:04:44 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:04:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95826f34968840372cf7395fcfeb007c4e01790028cbf66abf9b71b1432c789f`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc337e144872087cec71f834b17427501f8ad018507f711542e59af8b4b4df5`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde282dc14f2040cce3455570b4a87db9206c4a9a86bffd5d4d9877702dac85`  
		Last Modified: Wed, 11 Nov 2020 23:58:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c126dd795a4db16a12293c1fe16e2d83a756751ede3f642912247cf604ce0590`  
		Last Modified: Wed, 11 Nov 2020 23:59:12 GMT  
		Size: 232.9 MB (232934220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334a0c987646cd690541030ac04aaac9110da344b8306b0eab1a942c39e31fc2`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04587b3ede5db86dd3ebc5b15d785a4dde8df15fe927369d7d03cf487cc8d2a6`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abffb6c89c52efc79520d15108209c678abdebd595d86168e105f06d718ca1`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:35b4c4f8ed0462222de9be676ceeb5a04cdb8db5806862949eb86b3a0caa0a48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:85c7da4f622f4905caf91ed9735baeeb94ff81b599276f8bf8f3fb0d60769baf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2620971455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e974ed52b4f6442ad7c96016e2150599c4edddc4e1a87680448e84e6605e0b3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:00:44 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 22:00:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 22:00:46 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:04:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:04:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:04:44 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:04:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95826f34968840372cf7395fcfeb007c4e01790028cbf66abf9b71b1432c789f`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc337e144872087cec71f834b17427501f8ad018507f711542e59af8b4b4df5`  
		Last Modified: Wed, 11 Nov 2020 23:58:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cde282dc14f2040cce3455570b4a87db9206c4a9a86bffd5d4d9877702dac85`  
		Last Modified: Wed, 11 Nov 2020 23:58:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c126dd795a4db16a12293c1fe16e2d83a756751ede3f642912247cf604ce0590`  
		Last Modified: Wed, 11 Nov 2020 23:59:12 GMT  
		Size: 232.9 MB (232934220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334a0c987646cd690541030ac04aaac9110da344b8306b0eab1a942c39e31fc2`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04587b3ede5db86dd3ebc5b15d785a4dde8df15fe927369d7d03cf487cc8d2a6`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abffb6c89c52efc79520d15108209c678abdebd595d86168e105f06d718ca1`  
		Last Modified: Wed, 11 Nov 2020 23:58:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0c53d3180b47bbb7e6dcf3730be4fc34620ddf32b759b6d4577273c7766ad565
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:e7889807b129cfaf8285e77b9d68e4628385dd168f1172512bb2d138a2aa5519
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004538921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c1e3f5b37cccdfd64d877da154a583ff28506ccd6786e064413ebd95dc3741`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:55:47 GMT
ENV MONGO_VERSION=4.0.20
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.20-signed.msi
# Wed, 11 Nov 2020 21:55:48 GMT
ENV MONGO_DOWNLOAD_SHA256=f7e29506ed39ee7c0116c192f7e65a61f7c7decbe4c723aa8c6343079f28a7bb
# Wed, 11 Nov 2020 22:00:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:00:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:00:36 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:00:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3403a8ab1a2424bec19f328e0c8db0f1b90652b0acd9a1ceb56249408b3360`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1df638978971ee88015ef27b2f87a7b7094581aee1cb17352555137d588205f`  
		Last Modified: Wed, 11 Nov 2020 23:57:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05cd9e2eddcc06ff31a4ba6144fbe9b4eb2346d4534c55d57ac51b4e6ecb39a`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4921d494bc15f503d642ab7d7bd1951410391f505ac5ac7239a9f42c199df47a`  
		Last Modified: Wed, 11 Nov 2020 23:58:13 GMT  
		Size: 234.0 MB (233972169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafd33cde1da5d5d72101e7ea30f212e37c77400cd9baa0b6d0229a9ca39617`  
		Last Modified: Wed, 11 Nov 2020 23:57:26 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87747aed14209c176447112dc7760d74d4e433819ab80e57aa039536971a9a0`  
		Last Modified: Wed, 11 Nov 2020 23:57:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dc1fbd73a047d45fdc7889b14d4d86e28944c52f76ffd74ccd0751667d0e46`  
		Last Modified: Wed, 11 Nov 2020 23:57:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:c206c0fed83fbb255dfe1fac6da6512b4dbbf6d217809e4b01245657bdb2995a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:74ae7e6bc9b39cc7e165f94b25b578be68a08d27ca9b1410de04ba74c9208b55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155307089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6fa3383f923c63fbffcaaf617f6f9d1b1a99b8f7fc2d3a5d8e25660e82b6e05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:18:23 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 23 Oct 2020 18:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:18:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 18:18:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 23 Oct 2020 18:18:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 18:18:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 18:19:18 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 23 Oct 2020 18:19:18 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 18:19:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 23 Oct 2020 18:19:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_MAJOR=4.0
# Fri, 23 Oct 2020 18:19:19 GMT
ENV MONGO_VERSION=4.0.20
# Fri, 23 Oct 2020 18:19:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 23 Oct 2020 18:19:37 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 23 Oct 2020 18:19:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 23 Oct 2020 18:19:38 GMT
VOLUME [/data/db /data/configdb]
# Fri, 23 Oct 2020 18:19:38 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:19:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 18:19:41 GMT
EXPOSE 27017
# Fri, 23 Oct 2020 18:19:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc37f645f1f92efc0d481e792e0fa91ea089f6b73d9fb792c96633805fda5d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42052a7ad84f4de60a92f03233d87e607d2175611a861941c9341c1123dc456d`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 2.9 MB (2903893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff6eda0f824a9018cac13d7660227ddd551ba5fbd37341dd9ae9266b8c40f`  
		Last Modified: Fri, 23 Oct 2020 18:20:07 GMT  
		Size: 1.3 MB (1305153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bec5181c8b8dade0165fa145f52be3abe9f3a25f36b6ee8df2ac5dd1b5542d`  
		Last Modified: Fri, 23 Oct 2020 18:20:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec910c91aca5d2a75b18c619421617ea9c7cefe356af64c77910c9ac0a43bf4`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9634ed1120c7427dc3759b0230a7fe9a5b68f948358a96953096df9d755395`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff92f0f12004cf265a929ce95459961d996cb583a835a6079e4eba75268eeb9`  
		Last Modified: Fri, 23 Oct 2020 18:20:45 GMT  
		Size: 105.3 MB (105262932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d45b107e15920f784057db5618b6be3631a7386ea89804ee4c76436dd1ff8b`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6695f173ad69f19dc1befcb49fd07f0afc1b5d38513ae91f4c4ac76cb1731754`  
		Last Modified: Fri, 23 Oct 2020 18:20:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:51b630ba0998bce10ff0d6427cc86863e7ba156e4aa02e95486a6323c217c765
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144197957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:824f07817668b9db05e258a08e96ca7d3c775514d2771f28a6447e13d0a4862f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 23 Oct 2020 18:20:23 GMT
ADD file:5611ef5e4a339aa780380c12e06ca701cb7f2392b12aa8a481278806abc2a17c in / 
# Fri, 23 Oct 2020 18:20:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:20:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 18:20:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:20:31 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 04:22:12 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 06 Nov 2020 04:22:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:22:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 06 Nov 2020 04:22:29 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 06 Nov 2020 04:23:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Nov 2020 04:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Nov 2020 04:23:58 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 06 Nov 2020 04:24:01 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 06 Nov 2020 04:24:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 06 Nov 2020 04:24:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:24:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 06 Nov 2020 04:24:04 GMT
ENV MONGO_MAJOR=4.0
# Fri, 06 Nov 2020 04:24:05 GMT
ENV MONGO_VERSION=4.0.20
# Fri, 06 Nov 2020 04:24:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 06 Nov 2020 04:24:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 06 Nov 2020 04:24:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 06 Nov 2020 04:24:34 GMT
VOLUME [/data/db /data/configdb]
# Fri, 06 Nov 2020 04:24:34 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 06 Nov 2020 04:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Nov 2020 04:24:36 GMT
EXPOSE 27017
# Fri, 06 Nov 2020 04:24:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d2a73c0bcd690b0c96f2917b855b4499d5b9f1c49f92a39f32b6840fa49fe74e`  
		Last Modified: Wed, 14 Oct 2020 15:58:06 GMT  
		Size: 40.8 MB (40818920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee81a9e6847a65206218a3b456bc136f8e38689ebb56cc9877d597a41bb371`  
		Last Modified: Fri, 23 Oct 2020 18:21:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489a564b05761b210f9a87ff4b2b1e232cdd89eaaffd5e27bf658d0956b1d57`  
		Last Modified: Fri, 23 Oct 2020 18:21:26 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c25910825cfb7d71977bb81419f287002fb712d755ec89fb9fb9f120e30936`  
		Last Modified: Fri, 23 Oct 2020 18:21:27 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331f7652ae50a7ecee1b38efc4229d5c8e18267be16199bb5d0b49010415b83`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfefba0b0e1b8077dd4258e500120a3cc0132595641680e26c2a3e85d30bd239`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 2.4 MB (2447226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb9c59fba5eca90b7a641599724c7d89ae5b6612456c13c0d2db8b6680b2c8`  
		Last Modified: Fri, 06 Nov 2020 04:25:15 GMT  
		Size: 1.2 MB (1232119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363f9928931889afc6c2e4674bced6333375451e49357dd5fbb380e1c8028ea`  
		Last Modified: Fri, 06 Nov 2020 04:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a77d01a1b6e755afe6af91147d79c598f2ea7675b0c980e9490d298f853456`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2afa7111cdba2f4f7f4ce4ebce980756130241521a08a476b530d98951ef308`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2634e8ad74244d37ad47c2bc08072d3066d27b2bac633095126788621708b60d`  
		Last Modified: Fri, 06 Nov 2020 04:26:11 GMT  
		Size: 99.7 MB (99690270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae008ad37b51a3ff368222010a631a38d404723612c50e57a8abee888c99c4fe`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4293638312648ce4de297aa9d451ecd95bd89a915c77ff7f0091bbc728a3a2e`  
		Last Modified: Fri, 06 Nov 2020 04:25:46 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:73c0bd81c638e33ad8afd705330ad5addfa1df31b5c646dda6490ec2894f0977
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:2fc6a72a6e563f51f5fcc9e997eed996cec4db45aa0d415ff61928a9ecbbee95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164668474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2f1fdf242c8ff6a7ad1b2e00528a8995c8ba989b434093d91d815a2d750578`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:15 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 26 Sep 2020 01:03:16 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:17 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:17 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:17 GMT
ENV MONGO_MAJOR=4.2
# Fri, 02 Oct 2020 23:27:49 GMT
ENV MONGO_VERSION=4.2.10
# Fri, 02 Oct 2020 23:27:51 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 02 Oct 2020 23:28:25 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 02 Oct 2020 23:28:26 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 02 Oct 2020 23:28:27 GMT
VOLUME [/data/db /data/configdb]
# Fri, 02 Oct 2020 23:28:27 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 02 Oct 2020 23:28:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Oct 2020 23:28:28 GMT
EXPOSE 27017
# Fri, 02 Oct 2020 23:28:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3053f3c4c8fc9d449af2bb80a1118c8b227788b8c14c1dcd8d587425c924ef23`  
		Last Modified: Sat, 26 Sep 2020 01:05:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f678126aa385b0fa0171462c31562e8d2359efb4455aaee36616bd1b6f83a2fe`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f186b1372f71abfda437e8096c77ed28f056cbbe3d8d8bedba8292ceacec41`  
		Last Modified: Fri, 02 Oct 2020 23:29:37 GMT  
		Size: 129.2 MB (129156078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d12b46ad913f1cac1c3996b3aa7d1f2e987c76e922191b768bc8db0d3a7984b`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6aa707883c8a5f723d901a8b5f3c8e0c89d393679251b3d7d64f474d166e0ec`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cf4e7392f797d8c788c4725d240c685b595087ef6c1043e4ea4b311e232b8430
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154688504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f525bbc3460b50af6bc6414ab6c9db7fa18d2b6ad497ce87433f8e388baf49a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:21:38 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 25 Sep 2020 23:21:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:21:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:21:41 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:21:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:21:43 GMT
ENV MONGO_MAJOR=4.2
# Sat, 03 Oct 2020 00:19:47 GMT
ENV MONGO_VERSION=4.2.10
# Sat, 03 Oct 2020 00:19:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 03 Oct 2020 00:20:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 03 Oct 2020 00:20:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 03 Oct 2020 00:20:43 GMT
VOLUME [/data/db /data/configdb]
# Sat, 03 Oct 2020 00:20:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 03 Oct 2020 00:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Oct 2020 00:20:46 GMT
EXPOSE 27017
# Sat, 03 Oct 2020 00:20:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f6864862b6ebbde40c6fdbf7ce41be9d93114f91bf80fe245ebc1d4586184b`  
		Last Modified: Fri, 25 Sep 2020 23:24:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc824748c27aebf837abc1f2988c04c7c24c0d81c1238faaffe31d29607ac4b1`  
		Last Modified: Sat, 03 Oct 2020 00:21:25 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7da4ea772eb253e979c521314a72bee71d8c225e415b272bee0b19a354966`  
		Last Modified: Sat, 03 Oct 2020 00:21:51 GMT  
		Size: 122.9 MB (122944235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a233feed6a52657ff8e708f1b39cdc3686432c70fc3ea3152096731f6f73082c`  
		Last Modified: Sat, 03 Oct 2020 00:21:26 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996d45f1e350b1ac1bf9821b4df22277883a849fe52996149d51a3e5f62b9525`  
		Last Modified: Sat, 03 Oct 2020 00:21:25 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:de0620b43101307921bc704b8ac95fed6b01de5ac548f6eeaa17093be4c5bd2e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6526795736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9002dfa0476e9d81c8986545acb4b29254f2d7fbb14300694c023b843460f3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:04:56 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:04:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:04:58 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:28:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:28:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:28:41 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41f5ab43050cb00c3526da0ef42974faaeb3819fa6b5418714de8aa0a90be21`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624d7acdee78f499b83c9ef8eeea6ab580f00d0e5524a10c509cf59f5ccbf6db`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b035cd0518726950b98c0d43b75a33f656546e37f846de5b184f529e2fe3f4`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208655e32dbb79e67da8dbc3f3b7c8c2542f8531b5c6d37b691520bc12b0012`  
		Last Modified: Thu, 12 Nov 2020 00:13:45 GMT  
		Size: 756.2 MB (756228968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d640e0ed22df0984c4a7a09468ab97eef7811fabc1439ab165bc5e6b94ba9f`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af3345cd7c15fc482b39238720a6e9352459c8d4af99e784debcbde5c41b9f0`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5481836076857ea67cf2f8d4ede18ba08cff457241ecf0a2a52f8e067d8878c`  
		Last Modified: Wed, 11 Nov 2020 23:59:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:01bbb0eaf49f024d769577862f29521dc99896f92149199ad8315727e1e51c3f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3143314358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ec6d282332470634b4f7d3caef431a033186519a513226b65977daa3a1b6e5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:28:49 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:53:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:53:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:53:42 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:53:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af6bdd4eb64399a7dae7716dd23818b22990842a9ec7d50cc22f9a4722204ac`  
		Last Modified: Thu, 12 Nov 2020 00:14:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57989933bb56cc10b5935873dfc7f23652fa359f190f9610ed07ff84c141db25`  
		Last Modified: Thu, 12 Nov 2020 00:14:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c51c4bee1a474e497ded8e672713221c1b8f84f8f696ee3c789cee676e796e`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ab1da6cd291e55eed98c5b0fd572b47558f9d6eaff622a961ea5b7c1815cf5`  
		Last Modified: Thu, 12 Nov 2020 00:33:06 GMT  
		Size: 755.3 MB (755277120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559156f91ebf301b0a8acbf69748cdf06d5db7902c55bbf314b577faf64f0cf7`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b13d3e951cd9471c2a90e0971635a10b63da486d743243c03e74653eb1c2265`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7570a4ab5c7ed48ef5d2a4d1b6ba41b7ccca4de534eefc1084cad044af3ffeb0`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.10`

```console
$ docker pull mongo@sha256:73c0bd81c638e33ad8afd705330ad5addfa1df31b5c646dda6490ec2894f0977
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.2.10` - linux; amd64

```console
$ docker pull mongo@sha256:2fc6a72a6e563f51f5fcc9e997eed996cec4db45aa0d415ff61928a9ecbbee95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164668474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2f1fdf242c8ff6a7ad1b2e00528a8995c8ba989b434093d91d815a2d750578`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:15 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 26 Sep 2020 01:03:16 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:17 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:17 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:17 GMT
ENV MONGO_MAJOR=4.2
# Fri, 02 Oct 2020 23:27:49 GMT
ENV MONGO_VERSION=4.2.10
# Fri, 02 Oct 2020 23:27:51 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 02 Oct 2020 23:28:25 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 02 Oct 2020 23:28:26 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 02 Oct 2020 23:28:27 GMT
VOLUME [/data/db /data/configdb]
# Fri, 02 Oct 2020 23:28:27 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 02 Oct 2020 23:28:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Oct 2020 23:28:28 GMT
EXPOSE 27017
# Fri, 02 Oct 2020 23:28:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3053f3c4c8fc9d449af2bb80a1118c8b227788b8c14c1dcd8d587425c924ef23`  
		Last Modified: Sat, 26 Sep 2020 01:05:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f678126aa385b0fa0171462c31562e8d2359efb4455aaee36616bd1b6f83a2fe`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f186b1372f71abfda437e8096c77ed28f056cbbe3d8d8bedba8292ceacec41`  
		Last Modified: Fri, 02 Oct 2020 23:29:37 GMT  
		Size: 129.2 MB (129156078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d12b46ad913f1cac1c3996b3aa7d1f2e987c76e922191b768bc8db0d3a7984b`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6aa707883c8a5f723d901a8b5f3c8e0c89d393679251b3d7d64f474d166e0ec`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.10` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cf4e7392f797d8c788c4725d240c685b595087ef6c1043e4ea4b311e232b8430
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154688504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f525bbc3460b50af6bc6414ab6c9db7fa18d2b6ad497ce87433f8e388baf49a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:21:38 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 25 Sep 2020 23:21:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:21:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:21:41 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:21:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:21:43 GMT
ENV MONGO_MAJOR=4.2
# Sat, 03 Oct 2020 00:19:47 GMT
ENV MONGO_VERSION=4.2.10
# Sat, 03 Oct 2020 00:19:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 03 Oct 2020 00:20:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 03 Oct 2020 00:20:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 03 Oct 2020 00:20:43 GMT
VOLUME [/data/db /data/configdb]
# Sat, 03 Oct 2020 00:20:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 03 Oct 2020 00:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Oct 2020 00:20:46 GMT
EXPOSE 27017
# Sat, 03 Oct 2020 00:20:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f6864862b6ebbde40c6fdbf7ce41be9d93114f91bf80fe245ebc1d4586184b`  
		Last Modified: Fri, 25 Sep 2020 23:24:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc824748c27aebf837abc1f2988c04c7c24c0d81c1238faaffe31d29607ac4b1`  
		Last Modified: Sat, 03 Oct 2020 00:21:25 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7da4ea772eb253e979c521314a72bee71d8c225e415b272bee0b19a354966`  
		Last Modified: Sat, 03 Oct 2020 00:21:51 GMT  
		Size: 122.9 MB (122944235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a233feed6a52657ff8e708f1b39cdc3686432c70fc3ea3152096731f6f73082c`  
		Last Modified: Sat, 03 Oct 2020 00:21:26 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996d45f1e350b1ac1bf9821b4df22277883a849fe52996149d51a3e5f62b9525`  
		Last Modified: Sat, 03 Oct 2020 00:21:25 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.10` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:de0620b43101307921bc704b8ac95fed6b01de5ac548f6eeaa17093be4c5bd2e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6526795736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9002dfa0476e9d81c8986545acb4b29254f2d7fbb14300694c023b843460f3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:04:56 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:04:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:04:58 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:28:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:28:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:28:41 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41f5ab43050cb00c3526da0ef42974faaeb3819fa6b5418714de8aa0a90be21`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624d7acdee78f499b83c9ef8eeea6ab580f00d0e5524a10c509cf59f5ccbf6db`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b035cd0518726950b98c0d43b75a33f656546e37f846de5b184f529e2fe3f4`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208655e32dbb79e67da8dbc3f3b7c8c2542f8531b5c6d37b691520bc12b0012`  
		Last Modified: Thu, 12 Nov 2020 00:13:45 GMT  
		Size: 756.2 MB (756228968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d640e0ed22df0984c4a7a09468ab97eef7811fabc1439ab165bc5e6b94ba9f`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af3345cd7c15fc482b39238720a6e9352459c8d4af99e784debcbde5c41b9f0`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5481836076857ea67cf2f8d4ede18ba08cff457241ecf0a2a52f8e067d8878c`  
		Last Modified: Wed, 11 Nov 2020 23:59:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.10` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:01bbb0eaf49f024d769577862f29521dc99896f92149199ad8315727e1e51c3f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3143314358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ec6d282332470634b4f7d3caef431a033186519a513226b65977daa3a1b6e5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:28:49 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:53:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:53:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:53:42 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:53:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af6bdd4eb64399a7dae7716dd23818b22990842a9ec7d50cc22f9a4722204ac`  
		Last Modified: Thu, 12 Nov 2020 00:14:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57989933bb56cc10b5935873dfc7f23652fa359f190f9610ed07ff84c141db25`  
		Last Modified: Thu, 12 Nov 2020 00:14:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c51c4bee1a474e497ded8e672713221c1b8f84f8f696ee3c789cee676e796e`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ab1da6cd291e55eed98c5b0fd572b47558f9d6eaff622a961ea5b7c1815cf5`  
		Last Modified: Thu, 12 Nov 2020 00:33:06 GMT  
		Size: 755.3 MB (755277120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559156f91ebf301b0a8acbf69748cdf06d5db7902c55bbf314b577faf64f0cf7`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b13d3e951cd9471c2a90e0971635a10b63da486d743243c03e74653eb1c2265`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7570a4ab5c7ed48ef5d2a4d1b6ba41b7ccca4de534eefc1084cad044af3ffeb0`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.10-bionic`

```console
$ docker pull mongo@sha256:a701ad3cceb92e222072de016f4d6e153096ccb9353942eb5f5b5aac660a43ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2.10-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:2fc6a72a6e563f51f5fcc9e997eed996cec4db45aa0d415ff61928a9ecbbee95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164668474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2f1fdf242c8ff6a7ad1b2e00528a8995c8ba989b434093d91d815a2d750578`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:15 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 26 Sep 2020 01:03:16 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:17 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:17 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:17 GMT
ENV MONGO_MAJOR=4.2
# Fri, 02 Oct 2020 23:27:49 GMT
ENV MONGO_VERSION=4.2.10
# Fri, 02 Oct 2020 23:27:51 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 02 Oct 2020 23:28:25 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 02 Oct 2020 23:28:26 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 02 Oct 2020 23:28:27 GMT
VOLUME [/data/db /data/configdb]
# Fri, 02 Oct 2020 23:28:27 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 02 Oct 2020 23:28:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Oct 2020 23:28:28 GMT
EXPOSE 27017
# Fri, 02 Oct 2020 23:28:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3053f3c4c8fc9d449af2bb80a1118c8b227788b8c14c1dcd8d587425c924ef23`  
		Last Modified: Sat, 26 Sep 2020 01:05:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f678126aa385b0fa0171462c31562e8d2359efb4455aaee36616bd1b6f83a2fe`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f186b1372f71abfda437e8096c77ed28f056cbbe3d8d8bedba8292ceacec41`  
		Last Modified: Fri, 02 Oct 2020 23:29:37 GMT  
		Size: 129.2 MB (129156078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d12b46ad913f1cac1c3996b3aa7d1f2e987c76e922191b768bc8db0d3a7984b`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6aa707883c8a5f723d901a8b5f3c8e0c89d393679251b3d7d64f474d166e0ec`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.10-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cf4e7392f797d8c788c4725d240c685b595087ef6c1043e4ea4b311e232b8430
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154688504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f525bbc3460b50af6bc6414ab6c9db7fa18d2b6ad497ce87433f8e388baf49a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:21:38 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 25 Sep 2020 23:21:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:21:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:21:41 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:21:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:21:43 GMT
ENV MONGO_MAJOR=4.2
# Sat, 03 Oct 2020 00:19:47 GMT
ENV MONGO_VERSION=4.2.10
# Sat, 03 Oct 2020 00:19:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 03 Oct 2020 00:20:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 03 Oct 2020 00:20:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 03 Oct 2020 00:20:43 GMT
VOLUME [/data/db /data/configdb]
# Sat, 03 Oct 2020 00:20:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 03 Oct 2020 00:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Oct 2020 00:20:46 GMT
EXPOSE 27017
# Sat, 03 Oct 2020 00:20:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f6864862b6ebbde40c6fdbf7ce41be9d93114f91bf80fe245ebc1d4586184b`  
		Last Modified: Fri, 25 Sep 2020 23:24:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc824748c27aebf837abc1f2988c04c7c24c0d81c1238faaffe31d29607ac4b1`  
		Last Modified: Sat, 03 Oct 2020 00:21:25 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7da4ea772eb253e979c521314a72bee71d8c225e415b272bee0b19a354966`  
		Last Modified: Sat, 03 Oct 2020 00:21:51 GMT  
		Size: 122.9 MB (122944235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a233feed6a52657ff8e708f1b39cdc3686432c70fc3ea3152096731f6f73082c`  
		Last Modified: Sat, 03 Oct 2020 00:21:26 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996d45f1e350b1ac1bf9821b4df22277883a849fe52996149d51a3e5f62b9525`  
		Last Modified: Sat, 03 Oct 2020 00:21:25 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.10-windowsservercore`

```console
$ docker pull mongo@sha256:c0ea8b96bd3f23360aa19ffbd9868bc7b5fd59a6f3dbcbf99e0e89db9ae6ceea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.2.10-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:de0620b43101307921bc704b8ac95fed6b01de5ac548f6eeaa17093be4c5bd2e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6526795736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9002dfa0476e9d81c8986545acb4b29254f2d7fbb14300694c023b843460f3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:04:56 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:04:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:04:58 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:28:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:28:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:28:41 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41f5ab43050cb00c3526da0ef42974faaeb3819fa6b5418714de8aa0a90be21`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624d7acdee78f499b83c9ef8eeea6ab580f00d0e5524a10c509cf59f5ccbf6db`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b035cd0518726950b98c0d43b75a33f656546e37f846de5b184f529e2fe3f4`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208655e32dbb79e67da8dbc3f3b7c8c2542f8531b5c6d37b691520bc12b0012`  
		Last Modified: Thu, 12 Nov 2020 00:13:45 GMT  
		Size: 756.2 MB (756228968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d640e0ed22df0984c4a7a09468ab97eef7811fabc1439ab165bc5e6b94ba9f`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af3345cd7c15fc482b39238720a6e9352459c8d4af99e784debcbde5c41b9f0`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5481836076857ea67cf2f8d4ede18ba08cff457241ecf0a2a52f8e067d8878c`  
		Last Modified: Wed, 11 Nov 2020 23:59:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.10-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:01bbb0eaf49f024d769577862f29521dc99896f92149199ad8315727e1e51c3f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3143314358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ec6d282332470634b4f7d3caef431a033186519a513226b65977daa3a1b6e5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:28:49 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:53:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:53:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:53:42 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:53:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af6bdd4eb64399a7dae7716dd23818b22990842a9ec7d50cc22f9a4722204ac`  
		Last Modified: Thu, 12 Nov 2020 00:14:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57989933bb56cc10b5935873dfc7f23652fa359f190f9610ed07ff84c141db25`  
		Last Modified: Thu, 12 Nov 2020 00:14:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c51c4bee1a474e497ded8e672713221c1b8f84f8f696ee3c789cee676e796e`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ab1da6cd291e55eed98c5b0fd572b47558f9d6eaff622a961ea5b7c1815cf5`  
		Last Modified: Thu, 12 Nov 2020 00:33:06 GMT  
		Size: 755.3 MB (755277120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559156f91ebf301b0a8acbf69748cdf06d5db7902c55bbf314b577faf64f0cf7`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b13d3e951cd9471c2a90e0971635a10b63da486d743243c03e74653eb1c2265`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7570a4ab5c7ed48ef5d2a4d1b6ba41b7ccca4de534eefc1084cad044af3ffeb0`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.10-windowsservercore-1809`

```console
$ docker pull mongo@sha256:1328a0721204e3985ed565426f490aeae625bd0de7a9eca3d35c9efe6da0277f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.2.10-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:01bbb0eaf49f024d769577862f29521dc99896f92149199ad8315727e1e51c3f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3143314358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ec6d282332470634b4f7d3caef431a033186519a513226b65977daa3a1b6e5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:28:49 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:53:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:53:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:53:42 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:53:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af6bdd4eb64399a7dae7716dd23818b22990842a9ec7d50cc22f9a4722204ac`  
		Last Modified: Thu, 12 Nov 2020 00:14:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57989933bb56cc10b5935873dfc7f23652fa359f190f9610ed07ff84c141db25`  
		Last Modified: Thu, 12 Nov 2020 00:14:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c51c4bee1a474e497ded8e672713221c1b8f84f8f696ee3c789cee676e796e`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ab1da6cd291e55eed98c5b0fd572b47558f9d6eaff622a961ea5b7c1815cf5`  
		Last Modified: Thu, 12 Nov 2020 00:33:06 GMT  
		Size: 755.3 MB (755277120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559156f91ebf301b0a8acbf69748cdf06d5db7902c55bbf314b577faf64f0cf7`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b13d3e951cd9471c2a90e0971635a10b63da486d743243c03e74653eb1c2265`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7570a4ab5c7ed48ef5d2a4d1b6ba41b7ccca4de534eefc1084cad044af3ffeb0`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.10-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:252eafcaeb310865ef77afeea9bebab0646a7b32051e8ef39935b748b6f8d5fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:4.2.10-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:de0620b43101307921bc704b8ac95fed6b01de5ac548f6eeaa17093be4c5bd2e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6526795736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9002dfa0476e9d81c8986545acb4b29254f2d7fbb14300694c023b843460f3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:04:56 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:04:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:04:58 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:28:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:28:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:28:41 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41f5ab43050cb00c3526da0ef42974faaeb3819fa6b5418714de8aa0a90be21`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624d7acdee78f499b83c9ef8eeea6ab580f00d0e5524a10c509cf59f5ccbf6db`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b035cd0518726950b98c0d43b75a33f656546e37f846de5b184f529e2fe3f4`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208655e32dbb79e67da8dbc3f3b7c8c2542f8531b5c6d37b691520bc12b0012`  
		Last Modified: Thu, 12 Nov 2020 00:13:45 GMT  
		Size: 756.2 MB (756228968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d640e0ed22df0984c4a7a09468ab97eef7811fabc1439ab165bc5e6b94ba9f`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af3345cd7c15fc482b39238720a6e9352459c8d4af99e784debcbde5c41b9f0`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5481836076857ea67cf2f8d4ede18ba08cff457241ecf0a2a52f8e067d8878c`  
		Last Modified: Wed, 11 Nov 2020 23:59:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:a701ad3cceb92e222072de016f4d6e153096ccb9353942eb5f5b5aac660a43ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:2fc6a72a6e563f51f5fcc9e997eed996cec4db45aa0d415ff61928a9ecbbee95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164668474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2f1fdf242c8ff6a7ad1b2e00528a8995c8ba989b434093d91d815a2d750578`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:15 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Sat, 26 Sep 2020 01:03:16 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:17 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:17 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:17 GMT
ENV MONGO_MAJOR=4.2
# Fri, 02 Oct 2020 23:27:49 GMT
ENV MONGO_VERSION=4.2.10
# Fri, 02 Oct 2020 23:27:51 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 02 Oct 2020 23:28:25 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 02 Oct 2020 23:28:26 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 02 Oct 2020 23:28:27 GMT
VOLUME [/data/db /data/configdb]
# Fri, 02 Oct 2020 23:28:27 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 02 Oct 2020 23:28:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Oct 2020 23:28:28 GMT
EXPOSE 27017
# Fri, 02 Oct 2020 23:28:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3053f3c4c8fc9d449af2bb80a1118c8b227788b8c14c1dcd8d587425c924ef23`  
		Last Modified: Sat, 26 Sep 2020 01:05:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f678126aa385b0fa0171462c31562e8d2359efb4455aaee36616bd1b6f83a2fe`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f186b1372f71abfda437e8096c77ed28f056cbbe3d8d8bedba8292ceacec41`  
		Last Modified: Fri, 02 Oct 2020 23:29:37 GMT  
		Size: 129.2 MB (129156078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d12b46ad913f1cac1c3996b3aa7d1f2e987c76e922191b768bc8db0d3a7984b`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6aa707883c8a5f723d901a8b5f3c8e0c89d393679251b3d7d64f474d166e0ec`  
		Last Modified: Fri, 02 Oct 2020 23:29:08 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cf4e7392f797d8c788c4725d240c685b595087ef6c1043e4ea4b311e232b8430
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154688504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f525bbc3460b50af6bc6414ab6c9db7fa18d2b6ad497ce87433f8e388baf49a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:21:38 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 25 Sep 2020 23:21:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:21:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:21:41 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:21:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:21:43 GMT
ENV MONGO_MAJOR=4.2
# Sat, 03 Oct 2020 00:19:47 GMT
ENV MONGO_VERSION=4.2.10
# Sat, 03 Oct 2020 00:19:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 03 Oct 2020 00:20:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 03 Oct 2020 00:20:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 03 Oct 2020 00:20:43 GMT
VOLUME [/data/db /data/configdb]
# Sat, 03 Oct 2020 00:20:44 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 03 Oct 2020 00:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Oct 2020 00:20:46 GMT
EXPOSE 27017
# Sat, 03 Oct 2020 00:20:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f6864862b6ebbde40c6fdbf7ce41be9d93114f91bf80fe245ebc1d4586184b`  
		Last Modified: Fri, 25 Sep 2020 23:24:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc824748c27aebf837abc1f2988c04c7c24c0d81c1238faaffe31d29607ac4b1`  
		Last Modified: Sat, 03 Oct 2020 00:21:25 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7da4ea772eb253e979c521314a72bee71d8c225e415b272bee0b19a354966`  
		Last Modified: Sat, 03 Oct 2020 00:21:51 GMT  
		Size: 122.9 MB (122944235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a233feed6a52657ff8e708f1b39cdc3686432c70fc3ea3152096731f6f73082c`  
		Last Modified: Sat, 03 Oct 2020 00:21:26 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996d45f1e350b1ac1bf9821b4df22277883a849fe52996149d51a3e5f62b9525`  
		Last Modified: Sat, 03 Oct 2020 00:21:25 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:c0ea8b96bd3f23360aa19ffbd9868bc7b5fd59a6f3dbcbf99e0e89db9ae6ceea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:de0620b43101307921bc704b8ac95fed6b01de5ac548f6eeaa17093be4c5bd2e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6526795736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9002dfa0476e9d81c8986545acb4b29254f2d7fbb14300694c023b843460f3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:04:56 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:04:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:04:58 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:28:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:28:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:28:41 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41f5ab43050cb00c3526da0ef42974faaeb3819fa6b5418714de8aa0a90be21`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624d7acdee78f499b83c9ef8eeea6ab580f00d0e5524a10c509cf59f5ccbf6db`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b035cd0518726950b98c0d43b75a33f656546e37f846de5b184f529e2fe3f4`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208655e32dbb79e67da8dbc3f3b7c8c2542f8531b5c6d37b691520bc12b0012`  
		Last Modified: Thu, 12 Nov 2020 00:13:45 GMT  
		Size: 756.2 MB (756228968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d640e0ed22df0984c4a7a09468ab97eef7811fabc1439ab165bc5e6b94ba9f`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af3345cd7c15fc482b39238720a6e9352459c8d4af99e784debcbde5c41b9f0`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5481836076857ea67cf2f8d4ede18ba08cff457241ecf0a2a52f8e067d8878c`  
		Last Modified: Wed, 11 Nov 2020 23:59:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:01bbb0eaf49f024d769577862f29521dc99896f92149199ad8315727e1e51c3f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3143314358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ec6d282332470634b4f7d3caef431a033186519a513226b65977daa3a1b6e5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:28:49 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:53:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:53:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:53:42 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:53:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af6bdd4eb64399a7dae7716dd23818b22990842a9ec7d50cc22f9a4722204ac`  
		Last Modified: Thu, 12 Nov 2020 00:14:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57989933bb56cc10b5935873dfc7f23652fa359f190f9610ed07ff84c141db25`  
		Last Modified: Thu, 12 Nov 2020 00:14:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c51c4bee1a474e497ded8e672713221c1b8f84f8f696ee3c789cee676e796e`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ab1da6cd291e55eed98c5b0fd572b47558f9d6eaff622a961ea5b7c1815cf5`  
		Last Modified: Thu, 12 Nov 2020 00:33:06 GMT  
		Size: 755.3 MB (755277120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559156f91ebf301b0a8acbf69748cdf06d5db7902c55bbf314b577faf64f0cf7`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b13d3e951cd9471c2a90e0971635a10b63da486d743243c03e74653eb1c2265`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7570a4ab5c7ed48ef5d2a4d1b6ba41b7ccca4de534eefc1084cad044af3ffeb0`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:1328a0721204e3985ed565426f490aeae625bd0de7a9eca3d35c9efe6da0277f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:01bbb0eaf49f024d769577862f29521dc99896f92149199ad8315727e1e51c3f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3143314358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ec6d282332470634b4f7d3caef431a033186519a513226b65977daa3a1b6e5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:28:48 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:28:49 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:53:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:53:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:53:42 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:53:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af6bdd4eb64399a7dae7716dd23818b22990842a9ec7d50cc22f9a4722204ac`  
		Last Modified: Thu, 12 Nov 2020 00:14:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57989933bb56cc10b5935873dfc7f23652fa359f190f9610ed07ff84c141db25`  
		Last Modified: Thu, 12 Nov 2020 00:14:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c51c4bee1a474e497ded8e672713221c1b8f84f8f696ee3c789cee676e796e`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ab1da6cd291e55eed98c5b0fd572b47558f9d6eaff622a961ea5b7c1815cf5`  
		Last Modified: Thu, 12 Nov 2020 00:33:06 GMT  
		Size: 755.3 MB (755277120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559156f91ebf301b0a8acbf69748cdf06d5db7902c55bbf314b577faf64f0cf7`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b13d3e951cd9471c2a90e0971635a10b63da486d743243c03e74653eb1c2265`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7570a4ab5c7ed48ef5d2a4d1b6ba41b7ccca4de534eefc1084cad044af3ffeb0`  
		Last Modified: Thu, 12 Nov 2020 00:14:10 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:252eafcaeb310865ef77afeea9bebab0646a7b32051e8ef39935b748b6f8d5fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:de0620b43101307921bc704b8ac95fed6b01de5ac548f6eeaa17093be4c5bd2e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6526795736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9002dfa0476e9d81c8986545acb4b29254f2d7fbb14300694c023b843460f3`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:04:56 GMT
ENV MONGO_VERSION=4.2.10
# Wed, 11 Nov 2020 22:04:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.10-signed.msi
# Wed, 11 Nov 2020 22:04:58 GMT
ENV MONGO_DOWNLOAD_SHA256=73bd155ae0a073acda0c4737b40733f5d84afcfbc985a6e61736076e0ef768a2
# Wed, 11 Nov 2020 22:28:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 22:28:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 22:28:41 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 22:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41f5ab43050cb00c3526da0ef42974faaeb3819fa6b5418714de8aa0a90be21`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624d7acdee78f499b83c9ef8eeea6ab580f00d0e5524a10c509cf59f5ccbf6db`  
		Last Modified: Wed, 11 Nov 2020 23:59:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b035cd0518726950b98c0d43b75a33f656546e37f846de5b184f529e2fe3f4`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208655e32dbb79e67da8dbc3f3b7c8c2542f8531b5c6d37b691520bc12b0012`  
		Last Modified: Thu, 12 Nov 2020 00:13:45 GMT  
		Size: 756.2 MB (756228968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d640e0ed22df0984c4a7a09468ab97eef7811fabc1439ab165bc5e6b94ba9f`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af3345cd7c15fc482b39238720a6e9352459c8d4af99e784debcbde5c41b9f0`  
		Last Modified: Wed, 11 Nov 2020 23:59:24 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5481836076857ea67cf2f8d4ede18ba08cff457241ecf0a2a52f8e067d8878c`  
		Last Modified: Wed, 11 Nov 2020 23:59:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4`

```console
$ docker pull mongo@sha256:ca31e7cf0ba12b6e7cdbf8b888a6c66f2a4351ad862e13390c9aa9e289d46701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.4` - linux; amd64

```console
$ docker pull mongo@sha256:31f6433f7cfcd2180483e40728cbf97142df1e85de36d80d75c93e5e7fe10405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177990635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0c2ff8d3620c0910832424efef02787214013b1c5b1d9dc9d87d638e2ceb71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:52 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 26 Sep 2020 01:03:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_MAJOR=4.4
# Sat, 26 Sep 2020 01:03:54 GMT
ENV MONGO_VERSION=4.4.1
# Sat, 26 Sep 2020 01:03:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 26 Sep 2020 01:04:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 26 Sep 2020 01:04:17 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 26 Sep 2020 01:04:17 GMT
VOLUME [/data/db /data/configdb]
# Sat, 26 Sep 2020 01:04:17 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 26 Sep 2020 01:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 01:04:17 GMT
EXPOSE 27017
# Sat, 26 Sep 2020 01:04:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8e9d469d838ebf98e71cb6b3b7f8e240f3211ff9a748c2dbff89e89a6fbeb`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69705b632494baffeba7f6c1c0a94fd5ee03db85c89dfa2eaac1c63b688f0430`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7daea26376d3196b89343320721e500e9391aef836c98a11e405734c38efc03`  
		Last Modified: Sat, 26 Sep 2020 01:06:21 GMT  
		Size: 142.5 MB (142478251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1f9e1fc7786860f32896276f7d77d09229f899e165348849e9916f6a60359`  
		Last Modified: Sat, 26 Sep 2020 01:06:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e65fe7ffd2b7653fff155ba55cbb8ae920f294f1b861a71758f176cf9eaa6`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:813ecaa78bf36de902579105aac27356b2a0bd876dcc6d7fdc977cf3898191e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167940515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811d532cf7eeb16c636343bc3e183c1db7fe8d887762b141e975f74e81481e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:22:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:22:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:22:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:22:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:22:36 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:22:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:23:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:23:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:23:12 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:23:13 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:23:14 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:23:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aec146ec81548df08b7b730fc041116e64f844464070486ee95f93a41de1f3`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215b86ffc2f95704af100aec2bfabdcb5745cc2339c548fee0353eafe414f9b`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11b0a6ff5a4354355c3588f66dcfb3b8716e4fe55dda70431b330cf7756b650`  
		Last Modified: Fri, 25 Sep 2020 23:25:58 GMT  
		Size: 136.2 MB (136196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f36a0aa04da4aa9dbc7ee2f91f1c1dbc63dad241d94dc7f0c13f54734627e4`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855fdd1e2165c9684a4cf42a775a55e4a0b49138a52fbd97c97fcb547fe773c`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 3.9 KB (3948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; s390x

```console
$ docker pull mongo@sha256:de1f653589e4153f89f7d242f907c69c16ea91f95f2a94240a19634aa8d57c4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172881569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc0c05512382652300ed10d809912071b8ee0ca14c10891cabccd8228c6dc94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:28:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:28:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:28:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:29:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:29:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:29:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:29:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:29:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:30:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:30:03 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:30:03 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:04 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:30:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288641caad70cb1c99ea2cd010ce53478a4fcde867a83434c8f98575f1fc90`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb83c3ffb783f1412239a892171b331eef5d68b65aae1a2c51c44619cacb1c0`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 2.7 MB (2704583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67c01a91968aa16935794fc7d52f7742b3359858bcfa36f033e3a9a8247e780`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 5.7 MB (5746126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf72d8578ae0c25477822fd40465d9f9f696e8178817341284280781fe545f9d`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f80311986b5ccb82ae38f1f7b88c67e49b6fc81534ef8984e5b2109064d6b`  
		Last Modified: Fri, 25 Sep 2020 23:30:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862844c0ef43cc7917b410c17cbcd9e60c83231627cae7f40aa92a521f4efb6`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ef58863de1fef5f933f4f05dd35e6f38ea3d1f491e4363a67c0b07db5afaa`  
		Last Modified: Fri, 25 Sep 2020 23:30:54 GMT  
		Size: 139.1 MB (139050035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36be598b0fb9cf5388c223afc27633dc987a84af1aa05cf185133ea8ce300bb8`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd583fd9ef05f53886b3c68b812186511fcd3b1ad1bcc98ca3f244eec4dc2e5`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.1`

```console
$ docker pull mongo@sha256:ca31e7cf0ba12b6e7cdbf8b888a6c66f2a4351ad862e13390c9aa9e289d46701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.4.1` - linux; amd64

```console
$ docker pull mongo@sha256:31f6433f7cfcd2180483e40728cbf97142df1e85de36d80d75c93e5e7fe10405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177990635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0c2ff8d3620c0910832424efef02787214013b1c5b1d9dc9d87d638e2ceb71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:52 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 26 Sep 2020 01:03:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_MAJOR=4.4
# Sat, 26 Sep 2020 01:03:54 GMT
ENV MONGO_VERSION=4.4.1
# Sat, 26 Sep 2020 01:03:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 26 Sep 2020 01:04:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 26 Sep 2020 01:04:17 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 26 Sep 2020 01:04:17 GMT
VOLUME [/data/db /data/configdb]
# Sat, 26 Sep 2020 01:04:17 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 26 Sep 2020 01:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 01:04:17 GMT
EXPOSE 27017
# Sat, 26 Sep 2020 01:04:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8e9d469d838ebf98e71cb6b3b7f8e240f3211ff9a748c2dbff89e89a6fbeb`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69705b632494baffeba7f6c1c0a94fd5ee03db85c89dfa2eaac1c63b688f0430`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7daea26376d3196b89343320721e500e9391aef836c98a11e405734c38efc03`  
		Last Modified: Sat, 26 Sep 2020 01:06:21 GMT  
		Size: 142.5 MB (142478251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1f9e1fc7786860f32896276f7d77d09229f899e165348849e9916f6a60359`  
		Last Modified: Sat, 26 Sep 2020 01:06:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e65fe7ffd2b7653fff155ba55cbb8ae920f294f1b861a71758f176cf9eaa6`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.1` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:813ecaa78bf36de902579105aac27356b2a0bd876dcc6d7fdc977cf3898191e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167940515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811d532cf7eeb16c636343bc3e183c1db7fe8d887762b141e975f74e81481e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:22:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:22:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:22:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:22:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:22:36 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:22:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:23:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:23:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:23:12 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:23:13 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:23:14 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:23:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aec146ec81548df08b7b730fc041116e64f844464070486ee95f93a41de1f3`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215b86ffc2f95704af100aec2bfabdcb5745cc2339c548fee0353eafe414f9b`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11b0a6ff5a4354355c3588f66dcfb3b8716e4fe55dda70431b330cf7756b650`  
		Last Modified: Fri, 25 Sep 2020 23:25:58 GMT  
		Size: 136.2 MB (136196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f36a0aa04da4aa9dbc7ee2f91f1c1dbc63dad241d94dc7f0c13f54734627e4`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855fdd1e2165c9684a4cf42a775a55e4a0b49138a52fbd97c97fcb547fe773c`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 3.9 KB (3948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.1` - linux; s390x

```console
$ docker pull mongo@sha256:de1f653589e4153f89f7d242f907c69c16ea91f95f2a94240a19634aa8d57c4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172881569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc0c05512382652300ed10d809912071b8ee0ca14c10891cabccd8228c6dc94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:28:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:28:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:28:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:29:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:29:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:29:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:29:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:29:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:30:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:30:03 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:30:03 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:04 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:30:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288641caad70cb1c99ea2cd010ce53478a4fcde867a83434c8f98575f1fc90`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb83c3ffb783f1412239a892171b331eef5d68b65aae1a2c51c44619cacb1c0`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 2.7 MB (2704583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67c01a91968aa16935794fc7d52f7742b3359858bcfa36f033e3a9a8247e780`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 5.7 MB (5746126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf72d8578ae0c25477822fd40465d9f9f696e8178817341284280781fe545f9d`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f80311986b5ccb82ae38f1f7b88c67e49b6fc81534ef8984e5b2109064d6b`  
		Last Modified: Fri, 25 Sep 2020 23:30:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862844c0ef43cc7917b410c17cbcd9e60c83231627cae7f40aa92a521f4efb6`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ef58863de1fef5f933f4f05dd35e6f38ea3d1f491e4363a67c0b07db5afaa`  
		Last Modified: Fri, 25 Sep 2020 23:30:54 GMT  
		Size: 139.1 MB (139050035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36be598b0fb9cf5388c223afc27633dc987a84af1aa05cf185133ea8ce300bb8`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd583fd9ef05f53886b3c68b812186511fcd3b1ad1bcc98ca3f244eec4dc2e5`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.1` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.1` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.1-bionic`

```console
$ docker pull mongo@sha256:ada11a11b2687fcaa0a58565679ffad590153a407bf7cee3622248ff0fac2c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.1-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:31f6433f7cfcd2180483e40728cbf97142df1e85de36d80d75c93e5e7fe10405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177990635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0c2ff8d3620c0910832424efef02787214013b1c5b1d9dc9d87d638e2ceb71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:52 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 26 Sep 2020 01:03:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_MAJOR=4.4
# Sat, 26 Sep 2020 01:03:54 GMT
ENV MONGO_VERSION=4.4.1
# Sat, 26 Sep 2020 01:03:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 26 Sep 2020 01:04:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 26 Sep 2020 01:04:17 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 26 Sep 2020 01:04:17 GMT
VOLUME [/data/db /data/configdb]
# Sat, 26 Sep 2020 01:04:17 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 26 Sep 2020 01:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 01:04:17 GMT
EXPOSE 27017
# Sat, 26 Sep 2020 01:04:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8e9d469d838ebf98e71cb6b3b7f8e240f3211ff9a748c2dbff89e89a6fbeb`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69705b632494baffeba7f6c1c0a94fd5ee03db85c89dfa2eaac1c63b688f0430`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7daea26376d3196b89343320721e500e9391aef836c98a11e405734c38efc03`  
		Last Modified: Sat, 26 Sep 2020 01:06:21 GMT  
		Size: 142.5 MB (142478251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1f9e1fc7786860f32896276f7d77d09229f899e165348849e9916f6a60359`  
		Last Modified: Sat, 26 Sep 2020 01:06:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e65fe7ffd2b7653fff155ba55cbb8ae920f294f1b861a71758f176cf9eaa6`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.1-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:813ecaa78bf36de902579105aac27356b2a0bd876dcc6d7fdc977cf3898191e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167940515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811d532cf7eeb16c636343bc3e183c1db7fe8d887762b141e975f74e81481e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:22:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:22:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:22:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:22:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:22:36 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:22:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:23:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:23:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:23:12 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:23:13 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:23:14 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:23:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aec146ec81548df08b7b730fc041116e64f844464070486ee95f93a41de1f3`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215b86ffc2f95704af100aec2bfabdcb5745cc2339c548fee0353eafe414f9b`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11b0a6ff5a4354355c3588f66dcfb3b8716e4fe55dda70431b330cf7756b650`  
		Last Modified: Fri, 25 Sep 2020 23:25:58 GMT  
		Size: 136.2 MB (136196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f36a0aa04da4aa9dbc7ee2f91f1c1dbc63dad241d94dc7f0c13f54734627e4`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855fdd1e2165c9684a4cf42a775a55e4a0b49138a52fbd97c97fcb547fe773c`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 3.9 KB (3948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.1-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:de1f653589e4153f89f7d242f907c69c16ea91f95f2a94240a19634aa8d57c4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172881569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc0c05512382652300ed10d809912071b8ee0ca14c10891cabccd8228c6dc94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:28:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:28:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:28:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:29:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:29:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:29:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:29:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:29:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:30:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:30:03 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:30:03 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:04 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:30:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288641caad70cb1c99ea2cd010ce53478a4fcde867a83434c8f98575f1fc90`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb83c3ffb783f1412239a892171b331eef5d68b65aae1a2c51c44619cacb1c0`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 2.7 MB (2704583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67c01a91968aa16935794fc7d52f7742b3359858bcfa36f033e3a9a8247e780`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 5.7 MB (5746126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf72d8578ae0c25477822fd40465d9f9f696e8178817341284280781fe545f9d`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f80311986b5ccb82ae38f1f7b88c67e49b6fc81534ef8984e5b2109064d6b`  
		Last Modified: Fri, 25 Sep 2020 23:30:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862844c0ef43cc7917b410c17cbcd9e60c83231627cae7f40aa92a521f4efb6`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ef58863de1fef5f933f4f05dd35e6f38ea3d1f491e4363a67c0b07db5afaa`  
		Last Modified: Fri, 25 Sep 2020 23:30:54 GMT  
		Size: 139.1 MB (139050035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36be598b0fb9cf5388c223afc27633dc987a84af1aa05cf185133ea8ce300bb8`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd583fd9ef05f53886b3c68b812186511fcd3b1ad1bcc98ca3f244eec4dc2e5`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.1-windowsservercore`

```console
$ docker pull mongo@sha256:3bf28d1ad689837347ca6da7d42d7a16f72039215da75e2b0d763128ecfd3969
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.4.1-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.1-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.1-windowsservercore-1809`

```console
$ docker pull mongo@sha256:404b3eae63d02d3c6a2760ed238db20e488cc94b243d25a3a6e8ca3c3b5c5c71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.4.1-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.1-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:e14fd4c954f6a8957168be58afe5565839cbb9a28f5afb109ef8a4fafc917929
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:4.4.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-bionic`

```console
$ docker pull mongo@sha256:ada11a11b2687fcaa0a58565679ffad590153a407bf7cee3622248ff0fac2c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:31f6433f7cfcd2180483e40728cbf97142df1e85de36d80d75c93e5e7fe10405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177990635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0c2ff8d3620c0910832424efef02787214013b1c5b1d9dc9d87d638e2ceb71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:52 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 26 Sep 2020 01:03:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_MAJOR=4.4
# Sat, 26 Sep 2020 01:03:54 GMT
ENV MONGO_VERSION=4.4.1
# Sat, 26 Sep 2020 01:03:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 26 Sep 2020 01:04:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 26 Sep 2020 01:04:17 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 26 Sep 2020 01:04:17 GMT
VOLUME [/data/db /data/configdb]
# Sat, 26 Sep 2020 01:04:17 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 26 Sep 2020 01:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 01:04:17 GMT
EXPOSE 27017
# Sat, 26 Sep 2020 01:04:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8e9d469d838ebf98e71cb6b3b7f8e240f3211ff9a748c2dbff89e89a6fbeb`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69705b632494baffeba7f6c1c0a94fd5ee03db85c89dfa2eaac1c63b688f0430`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7daea26376d3196b89343320721e500e9391aef836c98a11e405734c38efc03`  
		Last Modified: Sat, 26 Sep 2020 01:06:21 GMT  
		Size: 142.5 MB (142478251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1f9e1fc7786860f32896276f7d77d09229f899e165348849e9916f6a60359`  
		Last Modified: Sat, 26 Sep 2020 01:06:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e65fe7ffd2b7653fff155ba55cbb8ae920f294f1b861a71758f176cf9eaa6`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:813ecaa78bf36de902579105aac27356b2a0bd876dcc6d7fdc977cf3898191e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167940515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811d532cf7eeb16c636343bc3e183c1db7fe8d887762b141e975f74e81481e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:22:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:22:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:22:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:22:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:22:36 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:22:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:23:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:23:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:23:12 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:23:13 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:23:14 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:23:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aec146ec81548df08b7b730fc041116e64f844464070486ee95f93a41de1f3`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215b86ffc2f95704af100aec2bfabdcb5745cc2339c548fee0353eafe414f9b`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11b0a6ff5a4354355c3588f66dcfb3b8716e4fe55dda70431b330cf7756b650`  
		Last Modified: Fri, 25 Sep 2020 23:25:58 GMT  
		Size: 136.2 MB (136196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f36a0aa04da4aa9dbc7ee2f91f1c1dbc63dad241d94dc7f0c13f54734627e4`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855fdd1e2165c9684a4cf42a775a55e4a0b49138a52fbd97c97fcb547fe773c`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 3.9 KB (3948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:de1f653589e4153f89f7d242f907c69c16ea91f95f2a94240a19634aa8d57c4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172881569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc0c05512382652300ed10d809912071b8ee0ca14c10891cabccd8228c6dc94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:28:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:28:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:28:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:29:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:29:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:29:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:29:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:29:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:30:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:30:03 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:30:03 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:04 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:30:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288641caad70cb1c99ea2cd010ce53478a4fcde867a83434c8f98575f1fc90`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb83c3ffb783f1412239a892171b331eef5d68b65aae1a2c51c44619cacb1c0`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 2.7 MB (2704583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67c01a91968aa16935794fc7d52f7742b3359858bcfa36f033e3a9a8247e780`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 5.7 MB (5746126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf72d8578ae0c25477822fd40465d9f9f696e8178817341284280781fe545f9d`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f80311986b5ccb82ae38f1f7b88c67e49b6fc81534ef8984e5b2109064d6b`  
		Last Modified: Fri, 25 Sep 2020 23:30:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862844c0ef43cc7917b410c17cbcd9e60c83231627cae7f40aa92a521f4efb6`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ef58863de1fef5f933f4f05dd35e6f38ea3d1f491e4363a67c0b07db5afaa`  
		Last Modified: Fri, 25 Sep 2020 23:30:54 GMT  
		Size: 139.1 MB (139050035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36be598b0fb9cf5388c223afc27633dc987a84af1aa05cf185133ea8ce300bb8`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd583fd9ef05f53886b3c68b812186511fcd3b1ad1bcc98ca3f244eec4dc2e5`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore`

```console
$ docker pull mongo@sha256:3bf28d1ad689837347ca6da7d42d7a16f72039215da75e2b0d763128ecfd3969
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.4-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:404b3eae63d02d3c6a2760ed238db20e488cc94b243d25a3a6e8ca3c3b5c5c71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:4.4-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:e14fd4c954f6a8957168be58afe5565839cbb9a28f5afb109ef8a4fafc917929
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:ada11a11b2687fcaa0a58565679ffad590153a407bf7cee3622248ff0fac2c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:31f6433f7cfcd2180483e40728cbf97142df1e85de36d80d75c93e5e7fe10405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177990635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0c2ff8d3620c0910832424efef02787214013b1c5b1d9dc9d87d638e2ceb71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:52 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 26 Sep 2020 01:03:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_MAJOR=4.4
# Sat, 26 Sep 2020 01:03:54 GMT
ENV MONGO_VERSION=4.4.1
# Sat, 26 Sep 2020 01:03:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 26 Sep 2020 01:04:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 26 Sep 2020 01:04:17 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 26 Sep 2020 01:04:17 GMT
VOLUME [/data/db /data/configdb]
# Sat, 26 Sep 2020 01:04:17 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 26 Sep 2020 01:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 01:04:17 GMT
EXPOSE 27017
# Sat, 26 Sep 2020 01:04:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8e9d469d838ebf98e71cb6b3b7f8e240f3211ff9a748c2dbff89e89a6fbeb`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69705b632494baffeba7f6c1c0a94fd5ee03db85c89dfa2eaac1c63b688f0430`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7daea26376d3196b89343320721e500e9391aef836c98a11e405734c38efc03`  
		Last Modified: Sat, 26 Sep 2020 01:06:21 GMT  
		Size: 142.5 MB (142478251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1f9e1fc7786860f32896276f7d77d09229f899e165348849e9916f6a60359`  
		Last Modified: Sat, 26 Sep 2020 01:06:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e65fe7ffd2b7653fff155ba55cbb8ae920f294f1b861a71758f176cf9eaa6`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:813ecaa78bf36de902579105aac27356b2a0bd876dcc6d7fdc977cf3898191e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167940515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811d532cf7eeb16c636343bc3e183c1db7fe8d887762b141e975f74e81481e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:22:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:22:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:22:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:22:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:22:36 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:22:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:23:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:23:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:23:12 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:23:13 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:23:14 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:23:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aec146ec81548df08b7b730fc041116e64f844464070486ee95f93a41de1f3`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215b86ffc2f95704af100aec2bfabdcb5745cc2339c548fee0353eafe414f9b`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11b0a6ff5a4354355c3588f66dcfb3b8716e4fe55dda70431b330cf7756b650`  
		Last Modified: Fri, 25 Sep 2020 23:25:58 GMT  
		Size: 136.2 MB (136196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f36a0aa04da4aa9dbc7ee2f91f1c1dbc63dad241d94dc7f0c13f54734627e4`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855fdd1e2165c9684a4cf42a775a55e4a0b49138a52fbd97c97fcb547fe773c`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 3.9 KB (3948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:de1f653589e4153f89f7d242f907c69c16ea91f95f2a94240a19634aa8d57c4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172881569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc0c05512382652300ed10d809912071b8ee0ca14c10891cabccd8228c6dc94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:28:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:28:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:28:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:29:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:29:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:29:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:29:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:29:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:30:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:30:03 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:30:03 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:04 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:30:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288641caad70cb1c99ea2cd010ce53478a4fcde867a83434c8f98575f1fc90`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb83c3ffb783f1412239a892171b331eef5d68b65aae1a2c51c44619cacb1c0`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 2.7 MB (2704583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67c01a91968aa16935794fc7d52f7742b3359858bcfa36f033e3a9a8247e780`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 5.7 MB (5746126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf72d8578ae0c25477822fd40465d9f9f696e8178817341284280781fe545f9d`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f80311986b5ccb82ae38f1f7b88c67e49b6fc81534ef8984e5b2109064d6b`  
		Last Modified: Fri, 25 Sep 2020 23:30:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862844c0ef43cc7917b410c17cbcd9e60c83231627cae7f40aa92a521f4efb6`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ef58863de1fef5f933f4f05dd35e6f38ea3d1f491e4363a67c0b07db5afaa`  
		Last Modified: Fri, 25 Sep 2020 23:30:54 GMT  
		Size: 139.1 MB (139050035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36be598b0fb9cf5388c223afc27633dc987a84af1aa05cf185133ea8ce300bb8`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd583fd9ef05f53886b3c68b812186511fcd3b1ad1bcc98ca3f244eec4dc2e5`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:3bf28d1ad689837347ca6da7d42d7a16f72039215da75e2b0d763128ecfd3969
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:4-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:404b3eae63d02d3c6a2760ed238db20e488cc94b243d25a3a6e8ca3c3b5c5c71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:e14fd4c954f6a8957168be58afe5565839cbb9a28f5afb109ef8a4fafc917929
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:ada11a11b2687fcaa0a58565679ffad590153a407bf7cee3622248ff0fac2c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:31f6433f7cfcd2180483e40728cbf97142df1e85de36d80d75c93e5e7fe10405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177990635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0c2ff8d3620c0910832424efef02787214013b1c5b1d9dc9d87d638e2ceb71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:52 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 26 Sep 2020 01:03:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_MAJOR=4.4
# Sat, 26 Sep 2020 01:03:54 GMT
ENV MONGO_VERSION=4.4.1
# Sat, 26 Sep 2020 01:03:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 26 Sep 2020 01:04:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 26 Sep 2020 01:04:17 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 26 Sep 2020 01:04:17 GMT
VOLUME [/data/db /data/configdb]
# Sat, 26 Sep 2020 01:04:17 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 26 Sep 2020 01:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 01:04:17 GMT
EXPOSE 27017
# Sat, 26 Sep 2020 01:04:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8e9d469d838ebf98e71cb6b3b7f8e240f3211ff9a748c2dbff89e89a6fbeb`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69705b632494baffeba7f6c1c0a94fd5ee03db85c89dfa2eaac1c63b688f0430`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7daea26376d3196b89343320721e500e9391aef836c98a11e405734c38efc03`  
		Last Modified: Sat, 26 Sep 2020 01:06:21 GMT  
		Size: 142.5 MB (142478251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1f9e1fc7786860f32896276f7d77d09229f899e165348849e9916f6a60359`  
		Last Modified: Sat, 26 Sep 2020 01:06:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e65fe7ffd2b7653fff155ba55cbb8ae920f294f1b861a71758f176cf9eaa6`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:813ecaa78bf36de902579105aac27356b2a0bd876dcc6d7fdc977cf3898191e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167940515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811d532cf7eeb16c636343bc3e183c1db7fe8d887762b141e975f74e81481e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:22:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:22:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:22:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:22:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:22:36 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:22:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:23:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:23:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:23:12 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:23:13 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:23:14 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:23:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aec146ec81548df08b7b730fc041116e64f844464070486ee95f93a41de1f3`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215b86ffc2f95704af100aec2bfabdcb5745cc2339c548fee0353eafe414f9b`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11b0a6ff5a4354355c3588f66dcfb3b8716e4fe55dda70431b330cf7756b650`  
		Last Modified: Fri, 25 Sep 2020 23:25:58 GMT  
		Size: 136.2 MB (136196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f36a0aa04da4aa9dbc7ee2f91f1c1dbc63dad241d94dc7f0c13f54734627e4`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855fdd1e2165c9684a4cf42a775a55e4a0b49138a52fbd97c97fcb547fe773c`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 3.9 KB (3948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:de1f653589e4153f89f7d242f907c69c16ea91f95f2a94240a19634aa8d57c4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172881569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc0c05512382652300ed10d809912071b8ee0ca14c10891cabccd8228c6dc94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:28:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:28:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:28:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:29:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:29:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:29:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:29:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:29:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:30:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:30:03 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:30:03 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:04 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:30:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288641caad70cb1c99ea2cd010ce53478a4fcde867a83434c8f98575f1fc90`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb83c3ffb783f1412239a892171b331eef5d68b65aae1a2c51c44619cacb1c0`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 2.7 MB (2704583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67c01a91968aa16935794fc7d52f7742b3359858bcfa36f033e3a9a8247e780`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 5.7 MB (5746126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf72d8578ae0c25477822fd40465d9f9f696e8178817341284280781fe545f9d`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f80311986b5ccb82ae38f1f7b88c67e49b6fc81534ef8984e5b2109064d6b`  
		Last Modified: Fri, 25 Sep 2020 23:30:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862844c0ef43cc7917b410c17cbcd9e60c83231627cae7f40aa92a521f4efb6`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ef58863de1fef5f933f4f05dd35e6f38ea3d1f491e4363a67c0b07db5afaa`  
		Last Modified: Fri, 25 Sep 2020 23:30:54 GMT  
		Size: 139.1 MB (139050035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36be598b0fb9cf5388c223afc27633dc987a84af1aa05cf185133ea8ce300bb8`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd583fd9ef05f53886b3c68b812186511fcd3b1ad1bcc98ca3f244eec4dc2e5`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:ca31e7cf0ba12b6e7cdbf8b888a6c66f2a4351ad862e13390c9aa9e289d46701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:31f6433f7cfcd2180483e40728cbf97142df1e85de36d80d75c93e5e7fe10405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177990635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0c2ff8d3620c0910832424efef02787214013b1c5b1d9dc9d87d638e2ceb71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:02:51 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 26 Sep 2020 01:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:01 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 01:03:01 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 26 Sep 2020 01:03:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 01:03:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 01:03:52 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Sat, 26 Sep 2020 01:03:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 26 Sep 2020 01:03:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 26 Sep 2020 01:03:53 GMT
ENV MONGO_MAJOR=4.4
# Sat, 26 Sep 2020 01:03:54 GMT
ENV MONGO_VERSION=4.4.1
# Sat, 26 Sep 2020 01:03:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 26 Sep 2020 01:04:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 26 Sep 2020 01:04:17 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 26 Sep 2020 01:04:17 GMT
VOLUME [/data/db /data/configdb]
# Sat, 26 Sep 2020 01:04:17 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 26 Sep 2020 01:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 01:04:17 GMT
EXPOSE 27017
# Sat, 26 Sep 2020 01:04:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892787ca4521e0a85a595173187b463be25c2a2553602af54d49b1e0370a9dc5`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2d54757a5b0c81dcbc423ed468c533b04e1c8a69debe60ed90bde3e2ffd52`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 3.0 MB (2974679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7d90822f30433ad424e479785033fa4c7f497b8326715453a1b68d554ae8e`  
		Last Modified: Sat, 26 Sep 2020 01:05:35 GMT  
		Size: 5.8 MB (5827328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518d3776320a8f11f5e586959c91b4912cc2cbaecea1df78e93d7252619cad2`  
		Last Modified: Sat, 26 Sep 2020 01:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8e9d469d838ebf98e71cb6b3b7f8e240f3211ff9a748c2dbff89e89a6fbeb`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69705b632494baffeba7f6c1c0a94fd5ee03db85c89dfa2eaac1c63b688f0430`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7daea26376d3196b89343320721e500e9391aef836c98a11e405734c38efc03`  
		Last Modified: Sat, 26 Sep 2020 01:06:21 GMT  
		Size: 142.5 MB (142478251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d1f9e1fc7786860f32896276f7d77d09229f899e165348849e9916f6a60359`  
		Last Modified: Sat, 26 Sep 2020 01:06:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e65fe7ffd2b7653fff155ba55cbb8ae920f294f1b861a71758f176cf9eaa6`  
		Last Modified: Sat, 26 Sep 2020 01:05:57 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:813ecaa78bf36de902579105aac27356b2a0bd876dcc6d7fdc977cf3898191e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167940515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811d532cf7eeb16c636343bc3e183c1db7fe8d887762b141e975f74e81481e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:20:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:21:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:21:14 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:21:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:22:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:22:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:22:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:22:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:22:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:22:36 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:22:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:23:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:23:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:23:12 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:23:13 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:23:14 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:23:15 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd165aaa6cf837afe497c787183e126b24a1ef1bf403484f10928ba64c46639`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a920ac996f2b9527ded97e3730a6f389b34d4461d3a011e8a9d760fec20638bc`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 2.7 MB (2666255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b726ca9cb34a0b6364c01411cfc8cfa6958d113914018d18cba243d56c0d649b`  
		Last Modified: Fri, 25 Sep 2020 23:24:55 GMT  
		Size: 5.3 MB (5346293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c3d8694a6885ba4f1bdb65f527e085af3dc91039dd9b60a9af62ddc42b1d3`  
		Last Modified: Fri, 25 Sep 2020 23:24:54 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aec146ec81548df08b7b730fc041116e64f844464070486ee95f93a41de1f3`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215b86ffc2f95704af100aec2bfabdcb5745cc2339c548fee0353eafe414f9b`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11b0a6ff5a4354355c3588f66dcfb3b8716e4fe55dda70431b330cf7756b650`  
		Last Modified: Fri, 25 Sep 2020 23:25:58 GMT  
		Size: 136.2 MB (136196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f36a0aa04da4aa9dbc7ee2f91f1c1dbc63dad241d94dc7f0c13f54734627e4`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855fdd1e2165c9684a4cf42a775a55e4a0b49138a52fbd97c97fcb547fe773c`  
		Last Modified: Fri, 25 Sep 2020 23:25:24 GMT  
		Size: 3.9 KB (3948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:de1f653589e4153f89f7d242f907c69c16ea91f95f2a94240a19634aa8d57c4d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172881569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc0c05512382652300ed10d809912071b8ee0ca14c10891cabccd8228c6dc94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:28:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 25 Sep 2020 23:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:28:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:28:48 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 25 Sep 2020 23:29:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:29:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:29:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 25 Sep 2020 23:29:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_MAJOR=4.4
# Fri, 25 Sep 2020 23:29:39 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 25 Sep 2020 23:29:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 25 Sep 2020 23:29:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 25 Sep 2020 23:30:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 25 Sep 2020 23:30:03 GMT
VOLUME [/data/db /data/configdb]
# Fri, 25 Sep 2020 23:30:03 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:04 GMT
EXPOSE 27017
# Fri, 25 Sep 2020 23:30:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288641caad70cb1c99ea2cd010ce53478a4fcde867a83434c8f98575f1fc90`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb83c3ffb783f1412239a892171b331eef5d68b65aae1a2c51c44619cacb1c0`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 2.7 MB (2704583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67c01a91968aa16935794fc7d52f7742b3359858bcfa36f033e3a9a8247e780`  
		Last Modified: Fri, 25 Sep 2020 23:30:18 GMT  
		Size: 5.7 MB (5746126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf72d8578ae0c25477822fd40465d9f9f696e8178817341284280781fe545f9d`  
		Last Modified: Fri, 25 Sep 2020 23:30:17 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f80311986b5ccb82ae38f1f7b88c67e49b6fc81534ef8984e5b2109064d6b`  
		Last Modified: Fri, 25 Sep 2020 23:30:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862844c0ef43cc7917b410c17cbcd9e60c83231627cae7f40aa92a521f4efb6`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ef58863de1fef5f933f4f05dd35e6f38ea3d1f491e4363a67c0b07db5afaa`  
		Last Modified: Fri, 25 Sep 2020 23:30:54 GMT  
		Size: 139.1 MB (139050035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36be598b0fb9cf5388c223afc27633dc987a84af1aa05cf185133ea8ce300bb8`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd583fd9ef05f53886b3c68b812186511fcd3b1ad1bcc98ca3f244eec4dc2e5`  
		Last Modified: Fri, 25 Sep 2020 23:30:36 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:3bf28d1ad689837347ca6da7d42d7a16f72039215da75e2b0d763128ecfd3969
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64
	-	windows version 10.0.17763.1577; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:404b3eae63d02d3c6a2760ed238db20e488cc94b243d25a3a6e8ca3c3b5c5c71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:e14fd4c954f6a8957168be58afe5565839cbb9a28f5afb109ef8a4fafc917929
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:70d75c811e7119c272cc8bd6e250a19224744ce90994643cf3293e7bff92692e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6475787068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe638cb1d0025e616a7855e25851a033ec5c03bd41edb1a3f7668d0cd0e236`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 22:53:54 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 22:53:55 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:17:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:17:37 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:17:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab86ddd13517f3182bc4644a978d4006bcff36ed6c4ef8bac02024e8b5733d`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa688970b778895a997c594a29adce41a72c281f50d63151970cebb22dc0fce4`  
		Last Modified: Thu, 12 Nov 2020 00:33:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3617ae0e19f6fcfc6a0e2bb4fffb8a447d24b734a920dc3550010baa544dabe7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b1e84eedcb5c5cba13317d3a43dbe7b8263255b284eb8edddbe3512c1783f2`  
		Last Modified: Thu, 12 Nov 2020 00:36:51 GMT  
		Size: 705.2 MB (705220271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e096b7f868e06104fc73c8996e3fcc37d50e51541c1e7def5def3a7a2cc2250`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daa6221976aa651508667db7bc9b017fb1c9d6aa4903ddb76e8b928100c3458`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1515386e8590a0c8bd324cae2413945ab7e5fa010608ed8319d33ccc86a7d7`  
		Last Modified: Thu, 12 Nov 2020 00:33:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
