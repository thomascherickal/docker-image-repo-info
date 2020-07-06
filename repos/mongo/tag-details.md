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
-	[`mongo:4.0.19`](#mongo4019)
-	[`mongo:4.0.19-windowsservercore`](#mongo4019-windowsservercore)
-	[`mongo:4.0.19-windowsservercore-1809`](#mongo4019-windowsservercore-1809)
-	[`mongo:4.0.19-windowsservercore-ltsc2016`](#mongo4019-windowsservercore-ltsc2016)
-	[`mongo:4.0.19-xenial`](#mongo4019-xenial)
-	[`mongo:4.0-windowsservercore`](#mongo40-windowsservercore)
-	[`mongo:4.0-windowsservercore-1809`](#mongo40-windowsservercore-1809)
-	[`mongo:4.0-windowsservercore-ltsc2016`](#mongo40-windowsservercore-ltsc2016)
-	[`mongo:4.0-xenial`](#mongo40-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2.8`](#mongo428)
-	[`mongo:4.2.8-bionic`](#mongo428-bionic)
-	[`mongo:4.2.8-windowsservercore`](#mongo428-windowsservercore)
-	[`mongo:4.2.8-windowsservercore-1809`](#mongo428-windowsservercore-1809)
-	[`mongo:4.2.8-windowsservercore-ltsc2016`](#mongo428-windowsservercore-ltsc2016)
-	[`mongo:4.2-bionic`](#mongo42-bionic)
-	[`mongo:4.2-windowsservercore`](#mongo42-windowsservercore)
-	[`mongo:4.2-windowsservercore-1809`](#mongo42-windowsservercore-1809)
-	[`mongo:4.2-windowsservercore-ltsc2016`](#mongo42-windowsservercore-ltsc2016)
-	[`mongo:4.4.0-rc12`](#mongo440-rc12)
-	[`mongo:4.4.0-rc12-bionic`](#mongo440-rc12-bionic)
-	[`mongo:4.4.0-rc12-windowsservercore`](#mongo440-rc12-windowsservercore)
-	[`mongo:4.4.0-rc12-windowsservercore-1809`](#mongo440-rc12-windowsservercore-1809)
-	[`mongo:4.4.0-rc12-windowsservercore-ltsc2016`](#mongo440-rc12-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:3384bc1423ff0b0e3145a9670e7f86a9df113afcf3d5ebe9d5d368fd8a4b0aac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:0c23d932c3366557612715e226c17829ede1044243e54d5192b26bdbbb489ef0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (165963539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944c82bef68bc2ec6a58db644f36ac218304605605b3f65951c5f46e2da2d4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:02:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_MAJOR=3.6
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_VERSION=3.6.18
# Mon, 06 Jul 2020 22:02:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:29 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:30 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:02:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0dd4e894c20703a849e6ff0ec94f944c602d5297f79627162774139ac323dd`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deec49ff17059de399bb53621bd7b544d6fe020931cb377478e21c738d75e969`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0dafd5a1a6566f63e891bb636a24a5f978f1c01eb2cfe4099f15d1100c7f07`  
		Last Modified: Mon, 06 Jul 2020 22:05:04 GMT  
		Size: 117.4 MB (117370225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71058f7697baae1cab46658f5228d68de55bd64732f4c450fd76c3f8cbd0b8f`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da3126121dbb4c13c9986f0e19fbd1b6c42a4a42fd1c3be54bc904974257816`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:a14f1e7d0c8e74bca064fd79a7aa34a432a2f0cf2e61d4d33b352ce1a31e98d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155250052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20f80998fd08f33fc5181399f89cd067ac9d35d86b3a6063e6786fad946072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:23:20 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:23:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:23:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:23:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_MAJOR=3.6
# Wed, 17 Jun 2020 03:23:26 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 17 Jun 2020 03:23:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:23:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:24:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:24:02 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:24:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:24:11 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:24:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6273f1d75581a230d9c91081a565493238adf9a52da319953a73a76b5e1151`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f3ee35ed8257ac4b1418f6edd3afef970462f931e9b9380a4f575c8c21149f`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273a73ba7a8d6fa9adfa346c96a6a9394e0af69ff18311c8afbca3ea60d5e7c4`  
		Last Modified: Wed, 17 Jun 2020 03:30:27 GMT  
		Size: 111.6 MB (111572207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45023f72bd29157d7c5781691d982672ab51058905e1ce6a98173ebff45983`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e9c207cf6d3e2bf05e2d8139808a1e142a315d7067547c18467e3e2dc7b14`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:3384bc1423ff0b0e3145a9670e7f86a9df113afcf3d5ebe9d5d368fd8a4b0aac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:0c23d932c3366557612715e226c17829ede1044243e54d5192b26bdbbb489ef0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (165963539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944c82bef68bc2ec6a58db644f36ac218304605605b3f65951c5f46e2da2d4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:02:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_MAJOR=3.6
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_VERSION=3.6.18
# Mon, 06 Jul 2020 22:02:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:29 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:30 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:02:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0dd4e894c20703a849e6ff0ec94f944c602d5297f79627162774139ac323dd`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deec49ff17059de399bb53621bd7b544d6fe020931cb377478e21c738d75e969`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0dafd5a1a6566f63e891bb636a24a5f978f1c01eb2cfe4099f15d1100c7f07`  
		Last Modified: Mon, 06 Jul 2020 22:05:04 GMT  
		Size: 117.4 MB (117370225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71058f7697baae1cab46658f5228d68de55bd64732f4c450fd76c3f8cbd0b8f`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da3126121dbb4c13c9986f0e19fbd1b6c42a4a42fd1c3be54bc904974257816`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:a14f1e7d0c8e74bca064fd79a7aa34a432a2f0cf2e61d4d33b352ce1a31e98d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155250052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20f80998fd08f33fc5181399f89cd067ac9d35d86b3a6063e6786fad946072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:23:20 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:23:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:23:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:23:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_MAJOR=3.6
# Wed, 17 Jun 2020 03:23:26 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 17 Jun 2020 03:23:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:23:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:24:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:24:02 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:24:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:24:11 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:24:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6273f1d75581a230d9c91081a565493238adf9a52da319953a73a76b5e1151`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f3ee35ed8257ac4b1418f6edd3afef970462f931e9b9380a4f575c8c21149f`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273a73ba7a8d6fa9adfa346c96a6a9394e0af69ff18311c8afbca3ea60d5e7c4`  
		Last Modified: Wed, 17 Jun 2020 03:30:27 GMT  
		Size: 111.6 MB (111572207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45023f72bd29157d7c5781691d982672ab51058905e1ce6a98173ebff45983`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e9c207cf6d3e2bf05e2d8139808a1e142a315d7067547c18467e3e2dc7b14`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18`

```console
$ docker pull mongo@sha256:3384bc1423ff0b0e3145a9670e7f86a9df113afcf3d5ebe9d5d368fd8a4b0aac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:3.6.18` - linux; amd64

```console
$ docker pull mongo@sha256:0c23d932c3366557612715e226c17829ede1044243e54d5192b26bdbbb489ef0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (165963539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944c82bef68bc2ec6a58db644f36ac218304605605b3f65951c5f46e2da2d4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:02:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_MAJOR=3.6
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_VERSION=3.6.18
# Mon, 06 Jul 2020 22:02:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:29 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:30 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:02:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0dd4e894c20703a849e6ff0ec94f944c602d5297f79627162774139ac323dd`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deec49ff17059de399bb53621bd7b544d6fe020931cb377478e21c738d75e969`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0dafd5a1a6566f63e891bb636a24a5f978f1c01eb2cfe4099f15d1100c7f07`  
		Last Modified: Mon, 06 Jul 2020 22:05:04 GMT  
		Size: 117.4 MB (117370225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71058f7697baae1cab46658f5228d68de55bd64732f4c450fd76c3f8cbd0b8f`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da3126121dbb4c13c9986f0e19fbd1b6c42a4a42fd1c3be54bc904974257816`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:a14f1e7d0c8e74bca064fd79a7aa34a432a2f0cf2e61d4d33b352ce1a31e98d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155250052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20f80998fd08f33fc5181399f89cd067ac9d35d86b3a6063e6786fad946072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:23:20 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:23:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:23:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:23:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_MAJOR=3.6
# Wed, 17 Jun 2020 03:23:26 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 17 Jun 2020 03:23:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:23:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:24:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:24:02 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:24:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:24:11 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:24:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6273f1d75581a230d9c91081a565493238adf9a52da319953a73a76b5e1151`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f3ee35ed8257ac4b1418f6edd3afef970462f931e9b9380a4f575c8c21149f`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273a73ba7a8d6fa9adfa346c96a6a9394e0af69ff18311c8afbca3ea60d5e7c4`  
		Last Modified: Wed, 17 Jun 2020 03:30:27 GMT  
		Size: 111.6 MB (111572207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45023f72bd29157d7c5781691d982672ab51058905e1ce6a98173ebff45983`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e9c207cf6d3e2bf05e2d8139808a1e142a315d7067547c18467e3e2dc7b14`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18-windowsservercore`

```console
$ docker pull mongo@sha256:bbdbeee49f3b69d6ecb3874572ad67e790cd49ac36c8f98533e9b99b922c74f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:3.6.18-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18-windowsservercore-1809`

```console
$ docker pull mongo@sha256:168f93ffc37589489ff16a458b124925235e7342353261bbac8aaacf84e9cff3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:3.6.18-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:52630676efc96befa6e39413412ef130f145cdf478f6e886a6e8cc088ef1deb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:3.6.18-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.18-xenial`

```console
$ docker pull mongo@sha256:4510025c5a8f819d3d2659730f6cf283364cdd08b8f8958cdcd4246d5b6d4284
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.18-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:0c23d932c3366557612715e226c17829ede1044243e54d5192b26bdbbb489ef0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (165963539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944c82bef68bc2ec6a58db644f36ac218304605605b3f65951c5f46e2da2d4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:02:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_MAJOR=3.6
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_VERSION=3.6.18
# Mon, 06 Jul 2020 22:02:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:29 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:30 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:02:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0dd4e894c20703a849e6ff0ec94f944c602d5297f79627162774139ac323dd`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deec49ff17059de399bb53621bd7b544d6fe020931cb377478e21c738d75e969`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0dafd5a1a6566f63e891bb636a24a5f978f1c01eb2cfe4099f15d1100c7f07`  
		Last Modified: Mon, 06 Jul 2020 22:05:04 GMT  
		Size: 117.4 MB (117370225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71058f7697baae1cab46658f5228d68de55bd64732f4c450fd76c3f8cbd0b8f`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da3126121dbb4c13c9986f0e19fbd1b6c42a4a42fd1c3be54bc904974257816`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.18-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:a14f1e7d0c8e74bca064fd79a7aa34a432a2f0cf2e61d4d33b352ce1a31e98d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155250052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20f80998fd08f33fc5181399f89cd067ac9d35d86b3a6063e6786fad946072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:23:20 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:23:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:23:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:23:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_MAJOR=3.6
# Wed, 17 Jun 2020 03:23:26 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 17 Jun 2020 03:23:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:23:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:24:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:24:02 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:24:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:24:11 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:24:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6273f1d75581a230d9c91081a565493238adf9a52da319953a73a76b5e1151`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f3ee35ed8257ac4b1418f6edd3afef970462f931e9b9380a4f575c8c21149f`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273a73ba7a8d6fa9adfa346c96a6a9394e0af69ff18311c8afbca3ea60d5e7c4`  
		Last Modified: Wed, 17 Jun 2020 03:30:27 GMT  
		Size: 111.6 MB (111572207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45023f72bd29157d7c5781691d982672ab51058905e1ce6a98173ebff45983`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e9c207cf6d3e2bf05e2d8139808a1e142a315d7067547c18467e3e2dc7b14`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:bbdbeee49f3b69d6ecb3874572ad67e790cd49ac36c8f98533e9b99b922c74f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:168f93ffc37589489ff16a458b124925235e7342353261bbac8aaacf84e9cff3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:52630676efc96befa6e39413412ef130f145cdf478f6e886a6e8cc088ef1deb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:4510025c5a8f819d3d2659730f6cf283364cdd08b8f8958cdcd4246d5b6d4284
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:0c23d932c3366557612715e226c17829ede1044243e54d5192b26bdbbb489ef0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (165963539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944c82bef68bc2ec6a58db644f36ac218304605605b3f65951c5f46e2da2d4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:02:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_MAJOR=3.6
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_VERSION=3.6.18
# Mon, 06 Jul 2020 22:02:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:29 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:30 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:02:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0dd4e894c20703a849e6ff0ec94f944c602d5297f79627162774139ac323dd`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deec49ff17059de399bb53621bd7b544d6fe020931cb377478e21c738d75e969`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0dafd5a1a6566f63e891bb636a24a5f978f1c01eb2cfe4099f15d1100c7f07`  
		Last Modified: Mon, 06 Jul 2020 22:05:04 GMT  
		Size: 117.4 MB (117370225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71058f7697baae1cab46658f5228d68de55bd64732f4c450fd76c3f8cbd0b8f`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da3126121dbb4c13c9986f0e19fbd1b6c42a4a42fd1c3be54bc904974257816`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:a14f1e7d0c8e74bca064fd79a7aa34a432a2f0cf2e61d4d33b352ce1a31e98d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155250052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20f80998fd08f33fc5181399f89cd067ac9d35d86b3a6063e6786fad946072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:23:20 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:23:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:23:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:23:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_MAJOR=3.6
# Wed, 17 Jun 2020 03:23:26 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 17 Jun 2020 03:23:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:23:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:24:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:24:02 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:24:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:24:11 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:24:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6273f1d75581a230d9c91081a565493238adf9a52da319953a73a76b5e1151`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f3ee35ed8257ac4b1418f6edd3afef970462f931e9b9380a4f575c8c21149f`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273a73ba7a8d6fa9adfa346c96a6a9394e0af69ff18311c8afbca3ea60d5e7c4`  
		Last Modified: Wed, 17 Jun 2020 03:30:27 GMT  
		Size: 111.6 MB (111572207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45023f72bd29157d7c5781691d982672ab51058905e1ce6a98173ebff45983`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e9c207cf6d3e2bf05e2d8139808a1e142a315d7067547c18467e3e2dc7b14`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:bbdbeee49f3b69d6ecb3874572ad67e790cd49ac36c8f98533e9b99b922c74f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:3-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:168f93ffc37589489ff16a458b124925235e7342353261bbac8aaacf84e9cff3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:52630676efc96befa6e39413412ef130f145cdf478f6e886a6e8cc088ef1deb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:4510025c5a8f819d3d2659730f6cf283364cdd08b8f8958cdcd4246d5b6d4284
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:0c23d932c3366557612715e226c17829ede1044243e54d5192b26bdbbb489ef0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (165963539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944c82bef68bc2ec6a58db644f36ac218304605605b3f65951c5f46e2da2d4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:02:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:10 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_MAJOR=3.6
# Mon, 06 Jul 2020 22:02:11 GMT
ENV MONGO_VERSION=3.6.18
# Mon, 06 Jul 2020 22:02:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:29 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:30 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:02:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0dd4e894c20703a849e6ff0ec94f944c602d5297f79627162774139ac323dd`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deec49ff17059de399bb53621bd7b544d6fe020931cb377478e21c738d75e969`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0dafd5a1a6566f63e891bb636a24a5f978f1c01eb2cfe4099f15d1100c7f07`  
		Last Modified: Mon, 06 Jul 2020 22:05:04 GMT  
		Size: 117.4 MB (117370225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71058f7697baae1cab46658f5228d68de55bd64732f4c450fd76c3f8cbd0b8f`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da3126121dbb4c13c9986f0e19fbd1b6c42a4a42fd1c3be54bc904974257816`  
		Last Modified: Mon, 06 Jul 2020 22:04:44 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:a14f1e7d0c8e74bca064fd79a7aa34a432a2f0cf2e61d4d33b352ce1a31e98d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155250052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20f80998fd08f33fc5181399f89cd067ac9d35d86b3a6063e6786fad946072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:23:20 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:23:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:23:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:23:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:23:25 GMT
ENV MONGO_MAJOR=3.6
# Wed, 17 Jun 2020 03:23:26 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 17 Jun 2020 03:23:29 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:23:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:24:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:24:02 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:24:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:24:11 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:24:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6273f1d75581a230d9c91081a565493238adf9a52da319953a73a76b5e1151`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f3ee35ed8257ac4b1418f6edd3afef970462f931e9b9380a4f575c8c21149f`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273a73ba7a8d6fa9adfa346c96a6a9394e0af69ff18311c8afbca3ea60d5e7c4`  
		Last Modified: Wed, 17 Jun 2020 03:30:27 GMT  
		Size: 111.6 MB (111572207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45023f72bd29157d7c5781691d982672ab51058905e1ce6a98173ebff45983`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e9c207cf6d3e2bf05e2d8139808a1e142a315d7067547c18467e3e2dc7b14`  
		Last Modified: Wed, 17 Jun 2020 03:30:00 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:37047f9762ca311dc2c84883c199b984322b82fc38097ac39624a8b98b15884d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:94c26811b76f697fa9ed91431d3665cfc6d87254c7980ddf2510c55833700835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164659719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d11486a97a77beaad31f63463a744dc3070ed4070bd15a695898a171f349441`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:03:34 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 22:03:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:03:35 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:03:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 22:03:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:03:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:03:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:03:56 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:03:56 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:03:57 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b916e924f1778f3230a1b137a675f2e8be7000c8c85e63e1c6432bcaaf12b5`  
		Last Modified: Mon, 06 Jul 2020 22:05:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805b21b6014c2d2a6a6ec4196c020291a87385046ae71c50dbb266113315e17`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7775fed6386269ff74f698e1b016ac356ee5f2299e86d2ab1ab4f09456fe2735`  
		Last Modified: Mon, 06 Jul 2020 22:05:52 GMT  
		Size: 129.1 MB (129121934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94226c388074f114ce594ea4a972fbead3f892e931da7b6918393f5994be1778`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7bf6a32e97cd93a1351b98c52cc7518f0d0592b48ee15aa03d2dc08d42653`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cdec0bd28e60bc06892f9972803753d57fdc3d4bcff657b694ba7f35b80d3d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154677642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84af28ce3aa3b7b04964d7f7ee9eb0ae10e3c19e684ad29ceeca55c605f2924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:27:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 17 Jun 2020 03:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:27:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:27:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:19 GMT
ENV MONGO_MAJOR=4.2
# Wed, 17 Jun 2020 03:27:20 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 03:27:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:28:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:28:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:28:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:28:08 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:28:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2b58fe1082de604f779b26f7bac0f685326b5584f5a43457f1d51effdca86`  
		Last Modified: Wed, 17 Jun 2020 03:31:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52cb618aa3e851b5a35792b706fd4e70901c2e3fd1faa3fcf12d719ac3d8ff1`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8985f89f29dd85eccbd8da50a080817fa846f7b7baee89e54e83f79559fff4b`  
		Last Modified: Wed, 17 Jun 2020 03:31:35 GMT  
		Size: 122.9 MB (122900361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f01ca57315b3f1a9469f85034d0f072b2d67b5ee9d3c9d2e14e3487df4db4d`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414fc1b8d9a096289a531b03096d4af7478a1c627842175a15974cb041c879`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:fd127fabc1bf86887613c1468da9458cdc40911ecb2be77512c0eff1abab7fad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160601784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8f620c8146e13765df833a4b47d557436a720571e885a22723c1431b1e0692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 20:53:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 20:53:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:53:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:53:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:53:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:53:32 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:53:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:53:33 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:53:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58902fb585e4821ffa80bd89abeaa891bf6f300ea302d85c089768fb721eacc`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51829b8cf8dd38c72c0f94d87ff4af39d009f29247ca7c0e56ad482bf229f4e`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afc8f2fd906dff6030983b0b511c3de126fcdf5255f7a6f1682b4a6e97fd3a`  
		Last Modified: Mon, 06 Jul 2020 20:54:39 GMT  
		Size: 126.7 MB (126738005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1641f60d50a5f6029e584a560748712b711521aa9d0c1c87e91ef2a4cb32ea8c`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6c42abe7efd4b6acc1c8ce6b0aac98da4da44252eb5710466004737e77342`  
		Last Modified: Mon, 06 Jul 2020 20:54:40 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:858ab632b0161bf230f120e327b24f16ebf6b39a2ddb3b2171f4411f0ccd81a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:a30d0cf7fd5202699f6a9d3e136def4ad873ebdca2cadeb812466dd491acbc4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153847112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86451baf0c5189c7f1355d5648f2a8ab5b454e89c1b082d47429b2f5b0af193`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:37 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Mon, 06 Jul 2020 22:02:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:38 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:38 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_MAJOR=4.0
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_VERSION=4.0.19
# Mon, 06 Jul 2020 22:02:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:57 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:58 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:58 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:58 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:59 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f5a9c25422258532b0c7e6e49470cdad58ef538813118168739f4be35dff5a`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b171b1b0ecfde79f7d89e96183184d4b9be41c783ceaff7de14ce16426694b4e`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ab8d9ae3a3f13e7651a5106c5ca08f0f45adff32ef5e2489a604f2eda0cfb`  
		Last Modified: Mon, 06 Jul 2020 22:05:28 GMT  
		Size: 105.3 MB (105254367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00075ae3675f31f79b256fcf974beab1069ac18caaa812095af9657915f9ded`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0190dc7997c580a7209ec6f1d2059f5e69d68a865f181106c103edafd49a67c`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:2ceebfb3ba9dd87bee897485561b8c7b82065c0281127ab5f4782f38c2481d9c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143363263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cebd15eb77de47468757b975d4a261739eb155ba1e116c7dfe1bfa01bda91a22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:24:39 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 17 Jun 2020 03:24:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:24:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:24:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:24:45 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:24:46 GMT
ENV MONGO_MAJOR=4.0
# Wed, 17 Jun 2020 03:24:47 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 03:24:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:25:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:25:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:25:38 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:25:39 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:25:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:25:41 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:25:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fdd5271b26ffe0d62b29b25121931dcdbe6ebb7ea49ba6b24fd99e266112a`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd7739bdf8cd161542061f5bc73b8a6756dd8a561f9b8209a6d091aa4fcc503`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0483829d143872abb4f5eb93398b84d81da48055989fac0d4a17d73360ee5b`  
		Last Modified: Wed, 17 Jun 2020 03:31:01 GMT  
		Size: 99.7 MB (99685983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaee99aa1bb5266c3f49a40599712f23081844d6f9f1242a95e952fc787ed19`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6839344713a90022b7a568a420d74d75dab8bc2e7bf09a66fdb6c56ce063795e`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:1a3468a39b95b542655927d7e0a04353366dc703ded677e6c22451360c87bac9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6183054924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c053b22eb0ec81f93e0935c743ad67ebefcb1a5799d222cabaf3c11a513caffc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:14:52 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:14:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:14:54 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:32:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:32:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:32:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:32:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816499e8d3b97fdb4d8e47ee9d0d1f281a3b1eeb8850ff030523cff88380321e`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a589c682f9703eb3d409e2032c7919de1aefc19a3cb393b0c064eaef6f0be`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d73871c04674ed1c797392fe5bec4228f05654ebf5a6a58435036fb1abe2ee`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726d3ce65aa1b227ef614b059b137963db5ee0a8bc95a4a730d085a97fe6bc33`  
		Last Modified: Wed, 17 Jun 2020 01:30:29 GMT  
		Size: 449.0 MB (449049166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad0ff8e9f21a3c1e912d9eeeeb97ee2d5c553ee879ec5f5cccd0a184698a8a7`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f20c2735d1ba169d52da0302e523ab3b2c09d047ff177d330c3b6a1bd6026`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f51b73ffa29728a6caf389cb3cb091a7706b2ea1f1013eeace11097778c12`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:eb7fd8e0a8c3db95868d8e17bab4ac26092180248fc0b068cd15bc286cb2d083
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742131599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737ee931c2d9a8f5de2d151517486894b4a41d3b3339fbb6c2a6e0c65bedeccb`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:32:25 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:32:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:32:27 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:50:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:50:36 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:50:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a707c5dc762ba141d7a8cfbec6295f374527707f6eaf5c98abb2e978cfdd69c`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8348966f83fe75692293e65cfde9e25e61e57e47a99fde23ecd73642b2ff5b`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887dfff9dc52cbfb40b678f03ca01f03f8ac6c6d2d6ff0b5975d3a124bd1dc01`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de8a718850e42fbd3d5b80d7812a66349a84429e6723b9737fbdf391b6698c`  
		Last Modified: Wed, 17 Jun 2020 01:31:41 GMT  
		Size: 448.2 MB (448209541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111da423a065bc6ecad62ce7b9f223431a830dc2e9b4cb1648197242d7588792`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5bc7d4fd2ff019705f4be25c3f277871730c361ca588a58adff3b8e908cd2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80595cd8b92d2c1a9701d89839040895c7da7b2a27ecc9acc28d2784b311c1f2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.19`

```console
$ docker pull mongo@sha256:858ab632b0161bf230f120e327b24f16ebf6b39a2ddb3b2171f4411f0ccd81a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.0.19` - linux; amd64

```console
$ docker pull mongo@sha256:a30d0cf7fd5202699f6a9d3e136def4ad873ebdca2cadeb812466dd491acbc4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153847112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86451baf0c5189c7f1355d5648f2a8ab5b454e89c1b082d47429b2f5b0af193`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:37 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Mon, 06 Jul 2020 22:02:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:38 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:38 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_MAJOR=4.0
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_VERSION=4.0.19
# Mon, 06 Jul 2020 22:02:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:57 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:58 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:58 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:58 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:59 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f5a9c25422258532b0c7e6e49470cdad58ef538813118168739f4be35dff5a`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b171b1b0ecfde79f7d89e96183184d4b9be41c783ceaff7de14ce16426694b4e`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ab8d9ae3a3f13e7651a5106c5ca08f0f45adff32ef5e2489a604f2eda0cfb`  
		Last Modified: Mon, 06 Jul 2020 22:05:28 GMT  
		Size: 105.3 MB (105254367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00075ae3675f31f79b256fcf974beab1069ac18caaa812095af9657915f9ded`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0190dc7997c580a7209ec6f1d2059f5e69d68a865f181106c103edafd49a67c`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.19` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:2ceebfb3ba9dd87bee897485561b8c7b82065c0281127ab5f4782f38c2481d9c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143363263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cebd15eb77de47468757b975d4a261739eb155ba1e116c7dfe1bfa01bda91a22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:24:39 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 17 Jun 2020 03:24:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:24:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:24:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:24:45 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:24:46 GMT
ENV MONGO_MAJOR=4.0
# Wed, 17 Jun 2020 03:24:47 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 03:24:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:25:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:25:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:25:38 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:25:39 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:25:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:25:41 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:25:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fdd5271b26ffe0d62b29b25121931dcdbe6ebb7ea49ba6b24fd99e266112a`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd7739bdf8cd161542061f5bc73b8a6756dd8a561f9b8209a6d091aa4fcc503`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0483829d143872abb4f5eb93398b84d81da48055989fac0d4a17d73360ee5b`  
		Last Modified: Wed, 17 Jun 2020 03:31:01 GMT  
		Size: 99.7 MB (99685983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaee99aa1bb5266c3f49a40599712f23081844d6f9f1242a95e952fc787ed19`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6839344713a90022b7a568a420d74d75dab8bc2e7bf09a66fdb6c56ce063795e`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.19` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:1a3468a39b95b542655927d7e0a04353366dc703ded677e6c22451360c87bac9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6183054924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c053b22eb0ec81f93e0935c743ad67ebefcb1a5799d222cabaf3c11a513caffc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:14:52 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:14:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:14:54 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:32:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:32:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:32:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:32:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816499e8d3b97fdb4d8e47ee9d0d1f281a3b1eeb8850ff030523cff88380321e`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a589c682f9703eb3d409e2032c7919de1aefc19a3cb393b0c064eaef6f0be`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d73871c04674ed1c797392fe5bec4228f05654ebf5a6a58435036fb1abe2ee`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726d3ce65aa1b227ef614b059b137963db5ee0a8bc95a4a730d085a97fe6bc33`  
		Last Modified: Wed, 17 Jun 2020 01:30:29 GMT  
		Size: 449.0 MB (449049166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad0ff8e9f21a3c1e912d9eeeeb97ee2d5c553ee879ec5f5cccd0a184698a8a7`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f20c2735d1ba169d52da0302e523ab3b2c09d047ff177d330c3b6a1bd6026`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f51b73ffa29728a6caf389cb3cb091a7706b2ea1f1013eeace11097778c12`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.19` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:eb7fd8e0a8c3db95868d8e17bab4ac26092180248fc0b068cd15bc286cb2d083
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742131599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737ee931c2d9a8f5de2d151517486894b4a41d3b3339fbb6c2a6e0c65bedeccb`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:32:25 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:32:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:32:27 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:50:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:50:36 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:50:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a707c5dc762ba141d7a8cfbec6295f374527707f6eaf5c98abb2e978cfdd69c`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8348966f83fe75692293e65cfde9e25e61e57e47a99fde23ecd73642b2ff5b`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887dfff9dc52cbfb40b678f03ca01f03f8ac6c6d2d6ff0b5975d3a124bd1dc01`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de8a718850e42fbd3d5b80d7812a66349a84429e6723b9737fbdf391b6698c`  
		Last Modified: Wed, 17 Jun 2020 01:31:41 GMT  
		Size: 448.2 MB (448209541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111da423a065bc6ecad62ce7b9f223431a830dc2e9b4cb1648197242d7588792`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5bc7d4fd2ff019705f4be25c3f277871730c361ca588a58adff3b8e908cd2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80595cd8b92d2c1a9701d89839040895c7da7b2a27ecc9acc28d2784b311c1f2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.19-windowsservercore`

```console
$ docker pull mongo@sha256:228832407c9cfccf7c1c7820b2c8df88413ac75638d8db733fd8e94706097a11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.0.19-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:1a3468a39b95b542655927d7e0a04353366dc703ded677e6c22451360c87bac9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6183054924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c053b22eb0ec81f93e0935c743ad67ebefcb1a5799d222cabaf3c11a513caffc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:14:52 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:14:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:14:54 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:32:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:32:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:32:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:32:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816499e8d3b97fdb4d8e47ee9d0d1f281a3b1eeb8850ff030523cff88380321e`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a589c682f9703eb3d409e2032c7919de1aefc19a3cb393b0c064eaef6f0be`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d73871c04674ed1c797392fe5bec4228f05654ebf5a6a58435036fb1abe2ee`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726d3ce65aa1b227ef614b059b137963db5ee0a8bc95a4a730d085a97fe6bc33`  
		Last Modified: Wed, 17 Jun 2020 01:30:29 GMT  
		Size: 449.0 MB (449049166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad0ff8e9f21a3c1e912d9eeeeb97ee2d5c553ee879ec5f5cccd0a184698a8a7`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f20c2735d1ba169d52da0302e523ab3b2c09d047ff177d330c3b6a1bd6026`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f51b73ffa29728a6caf389cb3cb091a7706b2ea1f1013eeace11097778c12`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.19-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:eb7fd8e0a8c3db95868d8e17bab4ac26092180248fc0b068cd15bc286cb2d083
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742131599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737ee931c2d9a8f5de2d151517486894b4a41d3b3339fbb6c2a6e0c65bedeccb`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:32:25 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:32:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:32:27 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:50:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:50:36 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:50:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a707c5dc762ba141d7a8cfbec6295f374527707f6eaf5c98abb2e978cfdd69c`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8348966f83fe75692293e65cfde9e25e61e57e47a99fde23ecd73642b2ff5b`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887dfff9dc52cbfb40b678f03ca01f03f8ac6c6d2d6ff0b5975d3a124bd1dc01`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de8a718850e42fbd3d5b80d7812a66349a84429e6723b9737fbdf391b6698c`  
		Last Modified: Wed, 17 Jun 2020 01:31:41 GMT  
		Size: 448.2 MB (448209541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111da423a065bc6ecad62ce7b9f223431a830dc2e9b4cb1648197242d7588792`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5bc7d4fd2ff019705f4be25c3f277871730c361ca588a58adff3b8e908cd2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80595cd8b92d2c1a9701d89839040895c7da7b2a27ecc9acc28d2784b311c1f2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.19-windowsservercore-1809`

```console
$ docker pull mongo@sha256:758f3d74b248ca29c188aa7afe6af40107e685b039e4182fedca012d4e981702
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.0.19-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:eb7fd8e0a8c3db95868d8e17bab4ac26092180248fc0b068cd15bc286cb2d083
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742131599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737ee931c2d9a8f5de2d151517486894b4a41d3b3339fbb6c2a6e0c65bedeccb`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:32:25 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:32:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:32:27 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:50:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:50:36 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:50:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a707c5dc762ba141d7a8cfbec6295f374527707f6eaf5c98abb2e978cfdd69c`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8348966f83fe75692293e65cfde9e25e61e57e47a99fde23ecd73642b2ff5b`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887dfff9dc52cbfb40b678f03ca01f03f8ac6c6d2d6ff0b5975d3a124bd1dc01`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de8a718850e42fbd3d5b80d7812a66349a84429e6723b9737fbdf391b6698c`  
		Last Modified: Wed, 17 Jun 2020 01:31:41 GMT  
		Size: 448.2 MB (448209541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111da423a065bc6ecad62ce7b9f223431a830dc2e9b4cb1648197242d7588792`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5bc7d4fd2ff019705f4be25c3f277871730c361ca588a58adff3b8e908cd2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80595cd8b92d2c1a9701d89839040895c7da7b2a27ecc9acc28d2784b311c1f2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.19-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:bdf25441c3ae280bf10aa80c445d6eb90f76a8e2d288bfa13d2798aca90c85b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:4.0.19-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:1a3468a39b95b542655927d7e0a04353366dc703ded677e6c22451360c87bac9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6183054924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c053b22eb0ec81f93e0935c743ad67ebefcb1a5799d222cabaf3c11a513caffc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:14:52 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:14:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:14:54 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:32:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:32:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:32:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:32:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816499e8d3b97fdb4d8e47ee9d0d1f281a3b1eeb8850ff030523cff88380321e`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a589c682f9703eb3d409e2032c7919de1aefc19a3cb393b0c064eaef6f0be`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d73871c04674ed1c797392fe5bec4228f05654ebf5a6a58435036fb1abe2ee`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726d3ce65aa1b227ef614b059b137963db5ee0a8bc95a4a730d085a97fe6bc33`  
		Last Modified: Wed, 17 Jun 2020 01:30:29 GMT  
		Size: 449.0 MB (449049166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad0ff8e9f21a3c1e912d9eeeeb97ee2d5c553ee879ec5f5cccd0a184698a8a7`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f20c2735d1ba169d52da0302e523ab3b2c09d047ff177d330c3b6a1bd6026`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f51b73ffa29728a6caf389cb3cb091a7706b2ea1f1013eeace11097778c12`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.19-xenial`

```console
$ docker pull mongo@sha256:480d841313411013b0d0d0fccc7b1b2a59f0a965f230573c1c5777013e4d1dd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.19-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:a30d0cf7fd5202699f6a9d3e136def4ad873ebdca2cadeb812466dd491acbc4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153847112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86451baf0c5189c7f1355d5648f2a8ab5b454e89c1b082d47429b2f5b0af193`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:37 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Mon, 06 Jul 2020 22:02:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:38 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:38 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_MAJOR=4.0
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_VERSION=4.0.19
# Mon, 06 Jul 2020 22:02:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:57 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:58 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:58 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:58 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:59 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f5a9c25422258532b0c7e6e49470cdad58ef538813118168739f4be35dff5a`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b171b1b0ecfde79f7d89e96183184d4b9be41c783ceaff7de14ce16426694b4e`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ab8d9ae3a3f13e7651a5106c5ca08f0f45adff32ef5e2489a604f2eda0cfb`  
		Last Modified: Mon, 06 Jul 2020 22:05:28 GMT  
		Size: 105.3 MB (105254367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00075ae3675f31f79b256fcf974beab1069ac18caaa812095af9657915f9ded`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0190dc7997c580a7209ec6f1d2059f5e69d68a865f181106c103edafd49a67c`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.19-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:2ceebfb3ba9dd87bee897485561b8c7b82065c0281127ab5f4782f38c2481d9c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143363263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cebd15eb77de47468757b975d4a261739eb155ba1e116c7dfe1bfa01bda91a22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:24:39 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 17 Jun 2020 03:24:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:24:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:24:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:24:45 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:24:46 GMT
ENV MONGO_MAJOR=4.0
# Wed, 17 Jun 2020 03:24:47 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 03:24:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:25:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:25:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:25:38 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:25:39 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:25:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:25:41 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:25:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fdd5271b26ffe0d62b29b25121931dcdbe6ebb7ea49ba6b24fd99e266112a`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd7739bdf8cd161542061f5bc73b8a6756dd8a561f9b8209a6d091aa4fcc503`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0483829d143872abb4f5eb93398b84d81da48055989fac0d4a17d73360ee5b`  
		Last Modified: Wed, 17 Jun 2020 03:31:01 GMT  
		Size: 99.7 MB (99685983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaee99aa1bb5266c3f49a40599712f23081844d6f9f1242a95e952fc787ed19`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6839344713a90022b7a568a420d74d75dab8bc2e7bf09a66fdb6c56ce063795e`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:228832407c9cfccf7c1c7820b2c8df88413ac75638d8db733fd8e94706097a11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:1a3468a39b95b542655927d7e0a04353366dc703ded677e6c22451360c87bac9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6183054924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c053b22eb0ec81f93e0935c743ad67ebefcb1a5799d222cabaf3c11a513caffc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:14:52 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:14:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:14:54 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:32:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:32:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:32:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:32:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816499e8d3b97fdb4d8e47ee9d0d1f281a3b1eeb8850ff030523cff88380321e`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a589c682f9703eb3d409e2032c7919de1aefc19a3cb393b0c064eaef6f0be`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d73871c04674ed1c797392fe5bec4228f05654ebf5a6a58435036fb1abe2ee`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726d3ce65aa1b227ef614b059b137963db5ee0a8bc95a4a730d085a97fe6bc33`  
		Last Modified: Wed, 17 Jun 2020 01:30:29 GMT  
		Size: 449.0 MB (449049166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad0ff8e9f21a3c1e912d9eeeeb97ee2d5c553ee879ec5f5cccd0a184698a8a7`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f20c2735d1ba169d52da0302e523ab3b2c09d047ff177d330c3b6a1bd6026`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f51b73ffa29728a6caf389cb3cb091a7706b2ea1f1013eeace11097778c12`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:eb7fd8e0a8c3db95868d8e17bab4ac26092180248fc0b068cd15bc286cb2d083
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742131599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737ee931c2d9a8f5de2d151517486894b4a41d3b3339fbb6c2a6e0c65bedeccb`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:32:25 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:32:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:32:27 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:50:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:50:36 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:50:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a707c5dc762ba141d7a8cfbec6295f374527707f6eaf5c98abb2e978cfdd69c`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8348966f83fe75692293e65cfde9e25e61e57e47a99fde23ecd73642b2ff5b`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887dfff9dc52cbfb40b678f03ca01f03f8ac6c6d2d6ff0b5975d3a124bd1dc01`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de8a718850e42fbd3d5b80d7812a66349a84429e6723b9737fbdf391b6698c`  
		Last Modified: Wed, 17 Jun 2020 01:31:41 GMT  
		Size: 448.2 MB (448209541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111da423a065bc6ecad62ce7b9f223431a830dc2e9b4cb1648197242d7588792`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5bc7d4fd2ff019705f4be25c3f277871730c361ca588a58adff3b8e908cd2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80595cd8b92d2c1a9701d89839040895c7da7b2a27ecc9acc28d2784b311c1f2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:758f3d74b248ca29c188aa7afe6af40107e685b039e4182fedca012d4e981702
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:eb7fd8e0a8c3db95868d8e17bab4ac26092180248fc0b068cd15bc286cb2d083
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742131599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737ee931c2d9a8f5de2d151517486894b4a41d3b3339fbb6c2a6e0c65bedeccb`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:32:25 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:32:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:32:27 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:50:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:50:36 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:50:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a707c5dc762ba141d7a8cfbec6295f374527707f6eaf5c98abb2e978cfdd69c`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8348966f83fe75692293e65cfde9e25e61e57e47a99fde23ecd73642b2ff5b`  
		Last Modified: Wed, 17 Jun 2020 01:30:44 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887dfff9dc52cbfb40b678f03ca01f03f8ac6c6d2d6ff0b5975d3a124bd1dc01`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de8a718850e42fbd3d5b80d7812a66349a84429e6723b9737fbdf391b6698c`  
		Last Modified: Wed, 17 Jun 2020 01:31:41 GMT  
		Size: 448.2 MB (448209541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111da423a065bc6ecad62ce7b9f223431a830dc2e9b4cb1648197242d7588792`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5bc7d4fd2ff019705f4be25c3f277871730c361ca588a58adff3b8e908cd2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80595cd8b92d2c1a9701d89839040895c7da7b2a27ecc9acc28d2784b311c1f2`  
		Last Modified: Wed, 17 Jun 2020 01:30:42 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:bdf25441c3ae280bf10aa80c445d6eb90f76a8e2d288bfa13d2798aca90c85b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:1a3468a39b95b542655927d7e0a04353366dc703ded677e6c22451360c87bac9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6183054924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c053b22eb0ec81f93e0935c743ad67ebefcb1a5799d222cabaf3c11a513caffc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:14:52 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 00:14:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 17 Jun 2020 00:14:54 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 17 Jun 2020 00:32:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 00:32:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 00:32:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 00:32:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816499e8d3b97fdb4d8e47ee9d0d1f281a3b1eeb8850ff030523cff88380321e`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a589c682f9703eb3d409e2032c7919de1aefc19a3cb393b0c064eaef6f0be`  
		Last Modified: Wed, 17 Jun 2020 01:29:35 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d73871c04674ed1c797392fe5bec4228f05654ebf5a6a58435036fb1abe2ee`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726d3ce65aa1b227ef614b059b137963db5ee0a8bc95a4a730d085a97fe6bc33`  
		Last Modified: Wed, 17 Jun 2020 01:30:29 GMT  
		Size: 449.0 MB (449049166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad0ff8e9f21a3c1e912d9eeeeb97ee2d5c553ee879ec5f5cccd0a184698a8a7`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f20c2735d1ba169d52da0302e523ab3b2c09d047ff177d330c3b6a1bd6026`  
		Last Modified: Wed, 17 Jun 2020 01:29:32 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f51b73ffa29728a6caf389cb3cb091a7706b2ea1f1013eeace11097778c12`  
		Last Modified: Wed, 17 Jun 2020 01:29:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:480d841313411013b0d0d0fccc7b1b2a59f0a965f230573c1c5777013e4d1dd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:a30d0cf7fd5202699f6a9d3e136def4ad873ebdca2cadeb812466dd491acbc4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153847112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86451baf0c5189c7f1355d5648f2a8ab5b454e89c1b082d47429b2f5b0af193`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:01:33 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:01:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:01:47 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:02:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:02:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:02:37 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Mon, 06 Jul 2020 22:02:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:02:38 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:02:38 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_MAJOR=4.0
# Mon, 06 Jul 2020 22:02:39 GMT
ENV MONGO_VERSION=4.0.19
# Mon, 06 Jul 2020 22:02:40 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:02:57 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:02:58 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:02:58 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:02:58 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:02:59 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c46851587c4ab1367004b007028f7668494eed05cf4b744dea8e1621a2f90d`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95b502c9229e0d43a7ba420bd438a6b41699eb9ed43855576b22b2d6f843ee`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 2.9 MB (2904107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f61825667542b4d94cf29245725d4920c0b453f121871be8920713884c53f1`  
		Last Modified: Mon, 06 Jul 2020 22:04:46 GMT  
		Size: 1.3 MB (1305075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0b3847dd4f9dec902e431bb4f0e32055f0fb39ff30f9a5ce76a67a491d1a9`  
		Last Modified: Mon, 06 Jul 2020 22:04:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f5a9c25422258532b0c7e6e49470cdad58ef538813118168739f4be35dff5a`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b171b1b0ecfde79f7d89e96183184d4b9be41c783ceaff7de14ce16426694b4e`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ab8d9ae3a3f13e7651a5106c5ca08f0f45adff32ef5e2489a604f2eda0cfb`  
		Last Modified: Mon, 06 Jul 2020 22:05:28 GMT  
		Size: 105.3 MB (105254367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00075ae3675f31f79b256fcf974beab1069ac18caaa812095af9657915f9ded`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0190dc7997c580a7209ec6f1d2059f5e69d68a865f181106c103edafd49a67c`  
		Last Modified: Mon, 06 Jul 2020 22:05:10 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:2ceebfb3ba9dd87bee897485561b8c7b82065c0281127ab5f4782f38c2481d9c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143363263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cebd15eb77de47468757b975d4a261739eb155ba1e116c7dfe1bfa01bda91a22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:22:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:22:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:22:45 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:23:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:24:39 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 17 Jun 2020 03:24:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:24:43 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:24:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:24:45 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:24:46 GMT
ENV MONGO_MAJOR=4.0
# Wed, 17 Jun 2020 03:24:47 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 17 Jun 2020 03:24:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:25:33 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:25:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:25:38 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:25:39 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:25:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:25:41 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:25:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270afc1f069e440415e7f2ce6ea17182e6af8d92e4c8f67842fc4f54413d3b2e`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca9f74e6ca082c5da190f0f58ac30d4822b0ffd568394e5ffec26bb1fd6a07`  
		Last Modified: Wed, 17 Jun 2020 03:30:02 GMT  
		Size: 2.4 MB (2431869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567c330a76a757a4b3ad26abdef55c652ebb1e0e70b77b935d3afe42d59a499`  
		Last Modified: Wed, 17 Jun 2020 03:30:03 GMT  
		Size: 1.2 MB (1232045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e0ba58951fc1e9fa054b24cbd1cdab213c985e279cc76f8bf95465d62c50c`  
		Last Modified: Wed, 17 Jun 2020 03:30:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fdd5271b26ffe0d62b29b25121931dcdbe6ebb7ea49ba6b24fd99e266112a`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd7739bdf8cd161542061f5bc73b8a6756dd8a561f9b8209a6d091aa4fcc503`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0483829d143872abb4f5eb93398b84d81da48055989fac0d4a17d73360ee5b`  
		Last Modified: Wed, 17 Jun 2020 03:31:01 GMT  
		Size: 99.7 MB (99685983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaee99aa1bb5266c3f49a40599712f23081844d6f9f1242a95e952fc787ed19`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6839344713a90022b7a568a420d74d75dab8bc2e7bf09a66fdb6c56ce063795e`  
		Last Modified: Wed, 17 Jun 2020 03:30:36 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:37047f9762ca311dc2c84883c199b984322b82fc38097ac39624a8b98b15884d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:94c26811b76f697fa9ed91431d3665cfc6d87254c7980ddf2510c55833700835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164659719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d11486a97a77beaad31f63463a744dc3070ed4070bd15a695898a171f349441`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:03:34 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 22:03:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:03:35 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:03:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 22:03:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:03:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:03:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:03:56 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:03:56 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:03:57 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b916e924f1778f3230a1b137a675f2e8be7000c8c85e63e1c6432bcaaf12b5`  
		Last Modified: Mon, 06 Jul 2020 22:05:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805b21b6014c2d2a6a6ec4196c020291a87385046ae71c50dbb266113315e17`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7775fed6386269ff74f698e1b016ac356ee5f2299e86d2ab1ab4f09456fe2735`  
		Last Modified: Mon, 06 Jul 2020 22:05:52 GMT  
		Size: 129.1 MB (129121934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94226c388074f114ce594ea4a972fbead3f892e931da7b6918393f5994be1778`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7bf6a32e97cd93a1351b98c52cc7518f0d0592b48ee15aa03d2dc08d42653`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cdec0bd28e60bc06892f9972803753d57fdc3d4bcff657b694ba7f35b80d3d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154677642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84af28ce3aa3b7b04964d7f7ee9eb0ae10e3c19e684ad29ceeca55c605f2924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:27:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 17 Jun 2020 03:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:27:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:27:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:19 GMT
ENV MONGO_MAJOR=4.2
# Wed, 17 Jun 2020 03:27:20 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 03:27:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:28:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:28:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:28:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:28:08 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:28:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2b58fe1082de604f779b26f7bac0f685326b5584f5a43457f1d51effdca86`  
		Last Modified: Wed, 17 Jun 2020 03:31:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52cb618aa3e851b5a35792b706fd4e70901c2e3fd1faa3fcf12d719ac3d8ff1`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8985f89f29dd85eccbd8da50a080817fa846f7b7baee89e54e83f79559fff4b`  
		Last Modified: Wed, 17 Jun 2020 03:31:35 GMT  
		Size: 122.9 MB (122900361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f01ca57315b3f1a9469f85034d0f072b2d67b5ee9d3c9d2e14e3487df4db4d`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414fc1b8d9a096289a531b03096d4af7478a1c627842175a15974cb041c879`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; s390x

```console
$ docker pull mongo@sha256:fd127fabc1bf86887613c1468da9458cdc40911ecb2be77512c0eff1abab7fad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160601784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8f620c8146e13765df833a4b47d557436a720571e885a22723c1431b1e0692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 20:53:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 20:53:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:53:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:53:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:53:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:53:32 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:53:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:53:33 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:53:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58902fb585e4821ffa80bd89abeaa891bf6f300ea302d85c089768fb721eacc`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51829b8cf8dd38c72c0f94d87ff4af39d009f29247ca7c0e56ad482bf229f4e`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afc8f2fd906dff6030983b0b511c3de126fcdf5255f7a6f1682b4a6e97fd3a`  
		Last Modified: Mon, 06 Jul 2020 20:54:39 GMT  
		Size: 126.7 MB (126738005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1641f60d50a5f6029e584a560748712b711521aa9d0c1c87e91ef2a4cb32ea8c`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6c42abe7efd4b6acc1c8ce6b0aac98da4da44252eb5710466004737e77342`  
		Last Modified: Mon, 06 Jul 2020 20:54:40 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.8`

```console
$ docker pull mongo@sha256:37047f9762ca311dc2c84883c199b984322b82fc38097ac39624a8b98b15884d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.2.8` - linux; amd64

```console
$ docker pull mongo@sha256:94c26811b76f697fa9ed91431d3665cfc6d87254c7980ddf2510c55833700835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164659719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d11486a97a77beaad31f63463a744dc3070ed4070bd15a695898a171f349441`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:03:34 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 22:03:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:03:35 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:03:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 22:03:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:03:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:03:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:03:56 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:03:56 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:03:57 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b916e924f1778f3230a1b137a675f2e8be7000c8c85e63e1c6432bcaaf12b5`  
		Last Modified: Mon, 06 Jul 2020 22:05:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805b21b6014c2d2a6a6ec4196c020291a87385046ae71c50dbb266113315e17`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7775fed6386269ff74f698e1b016ac356ee5f2299e86d2ab1ab4f09456fe2735`  
		Last Modified: Mon, 06 Jul 2020 22:05:52 GMT  
		Size: 129.1 MB (129121934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94226c388074f114ce594ea4a972fbead3f892e931da7b6918393f5994be1778`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7bf6a32e97cd93a1351b98c52cc7518f0d0592b48ee15aa03d2dc08d42653`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.8` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cdec0bd28e60bc06892f9972803753d57fdc3d4bcff657b694ba7f35b80d3d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154677642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84af28ce3aa3b7b04964d7f7ee9eb0ae10e3c19e684ad29ceeca55c605f2924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:27:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 17 Jun 2020 03:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:27:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:27:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:19 GMT
ENV MONGO_MAJOR=4.2
# Wed, 17 Jun 2020 03:27:20 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 03:27:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:28:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:28:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:28:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:28:08 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:28:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2b58fe1082de604f779b26f7bac0f685326b5584f5a43457f1d51effdca86`  
		Last Modified: Wed, 17 Jun 2020 03:31:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52cb618aa3e851b5a35792b706fd4e70901c2e3fd1faa3fcf12d719ac3d8ff1`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8985f89f29dd85eccbd8da50a080817fa846f7b7baee89e54e83f79559fff4b`  
		Last Modified: Wed, 17 Jun 2020 03:31:35 GMT  
		Size: 122.9 MB (122900361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f01ca57315b3f1a9469f85034d0f072b2d67b5ee9d3c9d2e14e3487df4db4d`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414fc1b8d9a096289a531b03096d4af7478a1c627842175a15974cb041c879`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.8` - linux; s390x

```console
$ docker pull mongo@sha256:fd127fabc1bf86887613c1468da9458cdc40911ecb2be77512c0eff1abab7fad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160601784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8f620c8146e13765df833a4b47d557436a720571e885a22723c1431b1e0692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 20:53:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 20:53:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:53:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:53:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:53:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:53:32 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:53:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:53:33 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:53:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58902fb585e4821ffa80bd89abeaa891bf6f300ea302d85c089768fb721eacc`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51829b8cf8dd38c72c0f94d87ff4af39d009f29247ca7c0e56ad482bf229f4e`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afc8f2fd906dff6030983b0b511c3de126fcdf5255f7a6f1682b4a6e97fd3a`  
		Last Modified: Mon, 06 Jul 2020 20:54:39 GMT  
		Size: 126.7 MB (126738005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1641f60d50a5f6029e584a560748712b711521aa9d0c1c87e91ef2a4cb32ea8c`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6c42abe7efd4b6acc1c8ce6b0aac98da4da44252eb5710466004737e77342`  
		Last Modified: Mon, 06 Jul 2020 20:54:40 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.8` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.8` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.8-bionic`

```console
$ docker pull mongo@sha256:27721e00fde059507056a18d6b699ea3965941933ac2d01820ebdfaa88460f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2.8-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:94c26811b76f697fa9ed91431d3665cfc6d87254c7980ddf2510c55833700835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164659719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d11486a97a77beaad31f63463a744dc3070ed4070bd15a695898a171f349441`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:03:34 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 22:03:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:03:35 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:03:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 22:03:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:03:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:03:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:03:56 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:03:56 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:03:57 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b916e924f1778f3230a1b137a675f2e8be7000c8c85e63e1c6432bcaaf12b5`  
		Last Modified: Mon, 06 Jul 2020 22:05:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805b21b6014c2d2a6a6ec4196c020291a87385046ae71c50dbb266113315e17`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7775fed6386269ff74f698e1b016ac356ee5f2299e86d2ab1ab4f09456fe2735`  
		Last Modified: Mon, 06 Jul 2020 22:05:52 GMT  
		Size: 129.1 MB (129121934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94226c388074f114ce594ea4a972fbead3f892e931da7b6918393f5994be1778`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7bf6a32e97cd93a1351b98c52cc7518f0d0592b48ee15aa03d2dc08d42653`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.8-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cdec0bd28e60bc06892f9972803753d57fdc3d4bcff657b694ba7f35b80d3d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154677642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84af28ce3aa3b7b04964d7f7ee9eb0ae10e3c19e684ad29ceeca55c605f2924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:27:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 17 Jun 2020 03:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:27:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:27:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:19 GMT
ENV MONGO_MAJOR=4.2
# Wed, 17 Jun 2020 03:27:20 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 03:27:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:28:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:28:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:28:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:28:08 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:28:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2b58fe1082de604f779b26f7bac0f685326b5584f5a43457f1d51effdca86`  
		Last Modified: Wed, 17 Jun 2020 03:31:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52cb618aa3e851b5a35792b706fd4e70901c2e3fd1faa3fcf12d719ac3d8ff1`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8985f89f29dd85eccbd8da50a080817fa846f7b7baee89e54e83f79559fff4b`  
		Last Modified: Wed, 17 Jun 2020 03:31:35 GMT  
		Size: 122.9 MB (122900361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f01ca57315b3f1a9469f85034d0f072b2d67b5ee9d3c9d2e14e3487df4db4d`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414fc1b8d9a096289a531b03096d4af7478a1c627842175a15974cb041c879`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.8-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:fd127fabc1bf86887613c1468da9458cdc40911ecb2be77512c0eff1abab7fad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160601784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8f620c8146e13765df833a4b47d557436a720571e885a22723c1431b1e0692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 20:53:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 20:53:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:53:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:53:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:53:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:53:32 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:53:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:53:33 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:53:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58902fb585e4821ffa80bd89abeaa891bf6f300ea302d85c089768fb721eacc`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51829b8cf8dd38c72c0f94d87ff4af39d009f29247ca7c0e56ad482bf229f4e`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afc8f2fd906dff6030983b0b511c3de126fcdf5255f7a6f1682b4a6e97fd3a`  
		Last Modified: Mon, 06 Jul 2020 20:54:39 GMT  
		Size: 126.7 MB (126738005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1641f60d50a5f6029e584a560748712b711521aa9d0c1c87e91ef2a4cb32ea8c`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6c42abe7efd4b6acc1c8ce6b0aac98da4da44252eb5710466004737e77342`  
		Last Modified: Mon, 06 Jul 2020 20:54:40 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.8-windowsservercore`

```console
$ docker pull mongo@sha256:3dfacb1c248e30392bcfaba258677f7a057a4ea96b2a37de4839a01081742a64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.2.8-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.8-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.8-windowsservercore-1809`

```console
$ docker pull mongo@sha256:bc2bc28a30754135707bfc25dd73c4aceb4ae89c943a243433b0b3f321f640fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.2.8-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.8-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b6e497bdcaa3a451d4296f944c0a13ac07344a7879cb41fb387ae288308fc61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:4.2.8-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:27721e00fde059507056a18d6b699ea3965941933ac2d01820ebdfaa88460f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:94c26811b76f697fa9ed91431d3665cfc6d87254c7980ddf2510c55833700835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164659719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d11486a97a77beaad31f63463a744dc3070ed4070bd15a695898a171f349441`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:03:34 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 22:03:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:03:35 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:03:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 22:03:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:03:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:03:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:03:56 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:03:56 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:03:57 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b916e924f1778f3230a1b137a675f2e8be7000c8c85e63e1c6432bcaaf12b5`  
		Last Modified: Mon, 06 Jul 2020 22:05:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805b21b6014c2d2a6a6ec4196c020291a87385046ae71c50dbb266113315e17`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7775fed6386269ff74f698e1b016ac356ee5f2299e86d2ab1ab4f09456fe2735`  
		Last Modified: Mon, 06 Jul 2020 22:05:52 GMT  
		Size: 129.1 MB (129121934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94226c388074f114ce594ea4a972fbead3f892e931da7b6918393f5994be1778`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7bf6a32e97cd93a1351b98c52cc7518f0d0592b48ee15aa03d2dc08d42653`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cdec0bd28e60bc06892f9972803753d57fdc3d4bcff657b694ba7f35b80d3d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154677642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84af28ce3aa3b7b04964d7f7ee9eb0ae10e3c19e684ad29ceeca55c605f2924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:27:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 17 Jun 2020 03:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:27:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:27:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:19 GMT
ENV MONGO_MAJOR=4.2
# Wed, 17 Jun 2020 03:27:20 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 03:27:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:28:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:28:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:28:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:28:08 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:28:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2b58fe1082de604f779b26f7bac0f685326b5584f5a43457f1d51effdca86`  
		Last Modified: Wed, 17 Jun 2020 03:31:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52cb618aa3e851b5a35792b706fd4e70901c2e3fd1faa3fcf12d719ac3d8ff1`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8985f89f29dd85eccbd8da50a080817fa846f7b7baee89e54e83f79559fff4b`  
		Last Modified: Wed, 17 Jun 2020 03:31:35 GMT  
		Size: 122.9 MB (122900361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f01ca57315b3f1a9469f85034d0f072b2d67b5ee9d3c9d2e14e3487df4db4d`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414fc1b8d9a096289a531b03096d4af7478a1c627842175a15974cb041c879`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:fd127fabc1bf86887613c1468da9458cdc40911ecb2be77512c0eff1abab7fad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160601784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8f620c8146e13765df833a4b47d557436a720571e885a22723c1431b1e0692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 20:53:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 20:53:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:53:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:53:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:53:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:53:32 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:53:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:53:33 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:53:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58902fb585e4821ffa80bd89abeaa891bf6f300ea302d85c089768fb721eacc`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51829b8cf8dd38c72c0f94d87ff4af39d009f29247ca7c0e56ad482bf229f4e`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afc8f2fd906dff6030983b0b511c3de126fcdf5255f7a6f1682b4a6e97fd3a`  
		Last Modified: Mon, 06 Jul 2020 20:54:39 GMT  
		Size: 126.7 MB (126738005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1641f60d50a5f6029e584a560748712b711521aa9d0c1c87e91ef2a4cb32ea8c`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6c42abe7efd4b6acc1c8ce6b0aac98da4da44252eb5710466004737e77342`  
		Last Modified: Mon, 06 Jul 2020 20:54:40 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:3dfacb1c248e30392bcfaba258677f7a057a4ea96b2a37de4839a01081742a64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:bc2bc28a30754135707bfc25dd73c4aceb4ae89c943a243433b0b3f321f640fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b6e497bdcaa3a451d4296f944c0a13ac07344a7879cb41fb387ae288308fc61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-rc12`

```console
$ docker pull mongo@sha256:be3ad32c38a70fd492c9592af67fd24f37a3b1e1169e8b0eb8aad9df8f72585f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.4.0-rc12` - linux; amd64

```console
$ docker pull mongo@sha256:1f3d3a5056996ee2d79903b8b4bff07282c0509aa583ee5252808f360254eaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177734791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8d7e328853dd0862396362278bf2dd5eef370d694d03207a18f66204eed5a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:04:01 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:04:03 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:04:03 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:04:03 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:04:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:04:03 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 22:04:04 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 22:04:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:04:24 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:04:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:04:28 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:04:28 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:04:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:04:28 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:04:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d37d7cdfd1b41d0e0691ef4fb5a6bfa57c3c93586e8f8ad0d1e2a0c30ef33e4`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 6.3 KB (6255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d870a78a337f4bf08d119f39dca63af37bc4a1be41c2c4e490c0a963c7c0d`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fa6e90749b168660473aa9bb87538b7fe87ecb329dc7f074b4155d8086499`  
		Last Modified: Mon, 06 Jul 2020 22:06:20 GMT  
		Size: 142.2 MB (142192184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26368085ec6f36f53f5752930c4fca8f2f55ff73488f987b05eb9dd7a4acf2dc`  
		Last Modified: Mon, 06 Jul 2020 22:05:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f7e1b5994ab1fd1681edcbd0c5b1fdad271c456a9b6aee21a46509c9feef7`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 4.0 KB (3957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-rc12` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:d3cd6c066a6fd832500419862eb08ae7177239461bca46014901928156820139
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167718774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e57fa87b22dfb173515f25b7d36041fe6ef590d96574866680370cc4c1c9a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:28:31 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:28:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:28:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:28:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:28:41 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:28:42 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 20:41:41 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 20:41:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:42:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:42:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:42:45 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:42:46 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:42:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:42:47 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:42:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc22fb839309e0ff73d69148b1061567442476c00078e55fd8f2ca6fcd5c8`  
		Last Modified: Wed, 17 Jun 2020 03:31:47 GMT  
		Size: 6.3 KB (6253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f8978327ffb136a6c269d5dc77747e3ab023c8a6cc764d4245fe7c1e2bda67`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45f3afbd4755ff77072e256f3060cce5a18e8706317174784a0083750fe457e`  
		Last Modified: Mon, 06 Jul 2020 20:43:46 GMT  
		Size: 135.9 MB (135936675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1fb738b456ff8d587a791b61a9073840179d4ad43770e884614136adf99b6`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98555d93433808e042bcfd2219f52db76f2490128dfcfd100bfa8bb413544fc4`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-rc12` - linux; s390x

```console
$ docker pull mongo@sha256:46cd7bdac9a40b262a4551500c55506e432ab34ae10451c44ff0f43128bd3371
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172676863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f23234b61f437d2deff35ba0c81dc29750e02b2e053a8e3767e79ef1fd5156`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:38 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 20:53:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:40 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 20:53:41 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:54:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:54:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:54:06 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:54:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:54:06 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:54:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229cebbae25aab3e43b584e93b8164ce11270d4da12ef2f9982e34611a230f7c`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 6.3 KB (6256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5db194c8396d25a2f24c8f76f3dceff885a445d711e2f988022f89243776aa`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184278f82293893eabe0e0cba0bb7778e131c4266f5344a1e8838252bab102a4`  
		Last Modified: Mon, 06 Jul 2020 20:55:10 GMT  
		Size: 138.8 MB (138808255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023eb94e085651a2a59ce390e764a8525f6384a8921216af5b5c422ed968c0b9`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4c175205f706c518b3f76fda81975f61062bb4768384e77161c31bb573663`  
		Last Modified: Mon, 06 Jul 2020 20:54:52 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-rc12` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:109b4ab288adc65d76ce96e55b95f29fb0bbec55c94cc7229467011af2bce0e8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6147207021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17259ef535401aa2eecc5f71db8414001c57dd82218715ba4c640ce91e4115ba`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:35:02 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:35:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:35:04 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 19:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 19:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 19:53:31 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 19:53:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54ffbdaf3aadb6b317220cf4e92b11a6de1c5cb2cc18dfa65f0f74174289503`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850856c450c610fe936d4092b2601b2e51954d4c2911765fdcbacd35c9265e16`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d696a21e0be15b220b32f5f1573e4f255971a8f4a4c4b5058a3ab7c9a82b24d`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa1aa83d1aa5af76b31fc1e8d919c8630b9bdd3c8c985537a2d55d4e99632b`  
		Last Modified: Mon, 06 Jul 2020 20:14:32 GMT  
		Size: 413.2 MB (413201285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1110553f1f1924f90747aaa9041b000ae8821e1e66550514c67d3430e3911`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42d6bf1851c5d28ec6834c663101351f365a3a3a86169e31f91931f0233a853`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882c76b8dbdc7c09c1cfcf05d32aef3a22187b433540e1c1b6c46c2cafd669f5`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-rc12` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:45501c1c91bba37313926453272963f0d30585198e51f206fb47232f2f6587f9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706281586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed675ff78b678261819c48b8150aa58c2ed7438c3a1ddeea86f74a43d92a71be`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:53:51 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 20:12:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 20:12:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 20:12:44 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:12:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4105bf49a3822f93914d7ee327ff44c4ac6bd3debfc2f5a7e2503b0c74a115e9`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d4c23eb9a1980b7fa0e2c063608e605f66c02f5459d3a216f1efff25311756`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0ef9898a4f3618d2308567c35f45b4627d2f17ba5d3c962442ae03811db38`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439fc0f14bbfa308c62b45b50deafd6ee77a4c70b040578048ea39ad6561c507`  
		Last Modified: Mon, 06 Jul 2020 20:15:37 GMT  
		Size: 412.4 MB (412359286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178148d52549bf2f86d42b2bed2cccc94c868f503202cb9e8353edae309d85`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7515e1d305d903836d5c895f3e180ffd54f905c0e09a9dbad3af32115451ea6`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e156991efd8447da6e3f368487d5c61184e32995f0db909e0a3b3ba82d59a10`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-rc12-bionic`

```console
$ docker pull mongo@sha256:5e6a482a21dd96e46bf12a9a43e35141164df8c99d6749ffe66a79dc4c0d4c47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.0-rc12-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:1f3d3a5056996ee2d79903b8b4bff07282c0509aa583ee5252808f360254eaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177734791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8d7e328853dd0862396362278bf2dd5eef370d694d03207a18f66204eed5a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:04:01 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:04:03 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:04:03 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:04:03 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:04:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:04:03 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 22:04:04 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 22:04:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:04:24 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:04:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:04:28 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:04:28 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:04:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:04:28 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:04:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d37d7cdfd1b41d0e0691ef4fb5a6bfa57c3c93586e8f8ad0d1e2a0c30ef33e4`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 6.3 KB (6255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d870a78a337f4bf08d119f39dca63af37bc4a1be41c2c4e490c0a963c7c0d`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fa6e90749b168660473aa9bb87538b7fe87ecb329dc7f074b4155d8086499`  
		Last Modified: Mon, 06 Jul 2020 22:06:20 GMT  
		Size: 142.2 MB (142192184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26368085ec6f36f53f5752930c4fca8f2f55ff73488f987b05eb9dd7a4acf2dc`  
		Last Modified: Mon, 06 Jul 2020 22:05:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f7e1b5994ab1fd1681edcbd0c5b1fdad271c456a9b6aee21a46509c9feef7`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 4.0 KB (3957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-rc12-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:d3cd6c066a6fd832500419862eb08ae7177239461bca46014901928156820139
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167718774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e57fa87b22dfb173515f25b7d36041fe6ef590d96574866680370cc4c1c9a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:28:31 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:28:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:28:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:28:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:28:41 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:28:42 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 20:41:41 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 20:41:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:42:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:42:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:42:45 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:42:46 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:42:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:42:47 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:42:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc22fb839309e0ff73d69148b1061567442476c00078e55fd8f2ca6fcd5c8`  
		Last Modified: Wed, 17 Jun 2020 03:31:47 GMT  
		Size: 6.3 KB (6253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f8978327ffb136a6c269d5dc77747e3ab023c8a6cc764d4245fe7c1e2bda67`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45f3afbd4755ff77072e256f3060cce5a18e8706317174784a0083750fe457e`  
		Last Modified: Mon, 06 Jul 2020 20:43:46 GMT  
		Size: 135.9 MB (135936675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1fb738b456ff8d587a791b61a9073840179d4ad43770e884614136adf99b6`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98555d93433808e042bcfd2219f52db76f2490128dfcfd100bfa8bb413544fc4`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-rc12-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:46cd7bdac9a40b262a4551500c55506e432ab34ae10451c44ff0f43128bd3371
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172676863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f23234b61f437d2deff35ba0c81dc29750e02b2e053a8e3767e79ef1fd5156`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:38 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 20:53:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:40 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 20:53:41 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:54:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:54:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:54:06 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:54:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:54:06 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:54:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229cebbae25aab3e43b584e93b8164ce11270d4da12ef2f9982e34611a230f7c`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 6.3 KB (6256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5db194c8396d25a2f24c8f76f3dceff885a445d711e2f988022f89243776aa`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184278f82293893eabe0e0cba0bb7778e131c4266f5344a1e8838252bab102a4`  
		Last Modified: Mon, 06 Jul 2020 20:55:10 GMT  
		Size: 138.8 MB (138808255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023eb94e085651a2a59ce390e764a8525f6384a8921216af5b5c422ed968c0b9`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4c175205f706c518b3f76fda81975f61062bb4768384e77161c31bb573663`  
		Last Modified: Mon, 06 Jul 2020 20:54:52 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-rc12-windowsservercore`

```console
$ docker pull mongo@sha256:a06cac34470ae48d4542150fa06503a6f417781abb05d8aff635178bcee04361
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.4.0-rc12-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:109b4ab288adc65d76ce96e55b95f29fb0bbec55c94cc7229467011af2bce0e8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6147207021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17259ef535401aa2eecc5f71db8414001c57dd82218715ba4c640ce91e4115ba`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:35:02 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:35:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:35:04 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 19:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 19:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 19:53:31 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 19:53:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54ffbdaf3aadb6b317220cf4e92b11a6de1c5cb2cc18dfa65f0f74174289503`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850856c450c610fe936d4092b2601b2e51954d4c2911765fdcbacd35c9265e16`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d696a21e0be15b220b32f5f1573e4f255971a8f4a4c4b5058a3ab7c9a82b24d`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa1aa83d1aa5af76b31fc1e8d919c8630b9bdd3c8c985537a2d55d4e99632b`  
		Last Modified: Mon, 06 Jul 2020 20:14:32 GMT  
		Size: 413.2 MB (413201285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1110553f1f1924f90747aaa9041b000ae8821e1e66550514c67d3430e3911`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42d6bf1851c5d28ec6834c663101351f365a3a3a86169e31f91931f0233a853`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882c76b8dbdc7c09c1cfcf05d32aef3a22187b433540e1c1b6c46c2cafd669f5`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-rc12-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:45501c1c91bba37313926453272963f0d30585198e51f206fb47232f2f6587f9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706281586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed675ff78b678261819c48b8150aa58c2ed7438c3a1ddeea86f74a43d92a71be`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:53:51 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 20:12:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 20:12:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 20:12:44 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:12:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4105bf49a3822f93914d7ee327ff44c4ac6bd3debfc2f5a7e2503b0c74a115e9`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d4c23eb9a1980b7fa0e2c063608e605f66c02f5459d3a216f1efff25311756`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0ef9898a4f3618d2308567c35f45b4627d2f17ba5d3c962442ae03811db38`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439fc0f14bbfa308c62b45b50deafd6ee77a4c70b040578048ea39ad6561c507`  
		Last Modified: Mon, 06 Jul 2020 20:15:37 GMT  
		Size: 412.4 MB (412359286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178148d52549bf2f86d42b2bed2cccc94c868f503202cb9e8353edae309d85`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7515e1d305d903836d5c895f3e180ffd54f905c0e09a9dbad3af32115451ea6`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e156991efd8447da6e3f368487d5c61184e32995f0db909e0a3b3ba82d59a10`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-rc12-windowsservercore-1809`

```console
$ docker pull mongo@sha256:94224515f3dd271bfa26f9ce7b0c3037842376ed3d7c4b4939dcd8dcb127cda4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.4.0-rc12-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:45501c1c91bba37313926453272963f0d30585198e51f206fb47232f2f6587f9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706281586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed675ff78b678261819c48b8150aa58c2ed7438c3a1ddeea86f74a43d92a71be`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:53:51 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 20:12:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 20:12:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 20:12:44 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:12:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4105bf49a3822f93914d7ee327ff44c4ac6bd3debfc2f5a7e2503b0c74a115e9`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d4c23eb9a1980b7fa0e2c063608e605f66c02f5459d3a216f1efff25311756`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0ef9898a4f3618d2308567c35f45b4627d2f17ba5d3c962442ae03811db38`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439fc0f14bbfa308c62b45b50deafd6ee77a4c70b040578048ea39ad6561c507`  
		Last Modified: Mon, 06 Jul 2020 20:15:37 GMT  
		Size: 412.4 MB (412359286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178148d52549bf2f86d42b2bed2cccc94c868f503202cb9e8353edae309d85`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7515e1d305d903836d5c895f3e180ffd54f905c0e09a9dbad3af32115451ea6`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e156991efd8447da6e3f368487d5c61184e32995f0db909e0a3b3ba82d59a10`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-rc12-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:b1ba9f21ebd21d2627f9a72b1bd16263ba9f3940994a4ccfe05b2be1c6c3d4fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:4.4.0-rc12-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:109b4ab288adc65d76ce96e55b95f29fb0bbec55c94cc7229467011af2bce0e8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6147207021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17259ef535401aa2eecc5f71db8414001c57dd82218715ba4c640ce91e4115ba`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:35:02 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:35:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:35:04 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 19:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 19:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 19:53:31 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 19:53:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54ffbdaf3aadb6b317220cf4e92b11a6de1c5cb2cc18dfa65f0f74174289503`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850856c450c610fe936d4092b2601b2e51954d4c2911765fdcbacd35c9265e16`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d696a21e0be15b220b32f5f1573e4f255971a8f4a4c4b5058a3ab7c9a82b24d`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa1aa83d1aa5af76b31fc1e8d919c8630b9bdd3c8c985537a2d55d4e99632b`  
		Last Modified: Mon, 06 Jul 2020 20:14:32 GMT  
		Size: 413.2 MB (413201285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1110553f1f1924f90747aaa9041b000ae8821e1e66550514c67d3430e3911`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42d6bf1851c5d28ec6834c663101351f365a3a3a86169e31f91931f0233a853`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882c76b8dbdc7c09c1cfcf05d32aef3a22187b433540e1c1b6c46c2cafd669f5`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc`

```console
$ docker pull mongo@sha256:be3ad32c38a70fd492c9592af67fd24f37a3b1e1169e8b0eb8aad9df8f72585f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.4-rc` - linux; amd64

```console
$ docker pull mongo@sha256:1f3d3a5056996ee2d79903b8b4bff07282c0509aa583ee5252808f360254eaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177734791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8d7e328853dd0862396362278bf2dd5eef370d694d03207a18f66204eed5a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:04:01 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:04:03 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:04:03 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:04:03 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:04:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:04:03 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 22:04:04 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 22:04:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:04:24 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:04:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:04:28 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:04:28 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:04:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:04:28 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:04:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d37d7cdfd1b41d0e0691ef4fb5a6bfa57c3c93586e8f8ad0d1e2a0c30ef33e4`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 6.3 KB (6255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d870a78a337f4bf08d119f39dca63af37bc4a1be41c2c4e490c0a963c7c0d`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fa6e90749b168660473aa9bb87538b7fe87ecb329dc7f074b4155d8086499`  
		Last Modified: Mon, 06 Jul 2020 22:06:20 GMT  
		Size: 142.2 MB (142192184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26368085ec6f36f53f5752930c4fca8f2f55ff73488f987b05eb9dd7a4acf2dc`  
		Last Modified: Mon, 06 Jul 2020 22:05:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f7e1b5994ab1fd1681edcbd0c5b1fdad271c456a9b6aee21a46509c9feef7`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 4.0 KB (3957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:d3cd6c066a6fd832500419862eb08ae7177239461bca46014901928156820139
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167718774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e57fa87b22dfb173515f25b7d36041fe6ef590d96574866680370cc4c1c9a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:28:31 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:28:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:28:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:28:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:28:41 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:28:42 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 20:41:41 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 20:41:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:42:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:42:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:42:45 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:42:46 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:42:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:42:47 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:42:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc22fb839309e0ff73d69148b1061567442476c00078e55fd8f2ca6fcd5c8`  
		Last Modified: Wed, 17 Jun 2020 03:31:47 GMT  
		Size: 6.3 KB (6253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f8978327ffb136a6c269d5dc77747e3ab023c8a6cc764d4245fe7c1e2bda67`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45f3afbd4755ff77072e256f3060cce5a18e8706317174784a0083750fe457e`  
		Last Modified: Mon, 06 Jul 2020 20:43:46 GMT  
		Size: 135.9 MB (135936675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1fb738b456ff8d587a791b61a9073840179d4ad43770e884614136adf99b6`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98555d93433808e042bcfd2219f52db76f2490128dfcfd100bfa8bb413544fc4`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc` - linux; s390x

```console
$ docker pull mongo@sha256:46cd7bdac9a40b262a4551500c55506e432ab34ae10451c44ff0f43128bd3371
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172676863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f23234b61f437d2deff35ba0c81dc29750e02b2e053a8e3767e79ef1fd5156`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:38 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 20:53:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:40 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 20:53:41 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:54:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:54:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:54:06 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:54:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:54:06 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:54:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229cebbae25aab3e43b584e93b8164ce11270d4da12ef2f9982e34611a230f7c`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 6.3 KB (6256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5db194c8396d25a2f24c8f76f3dceff885a445d711e2f988022f89243776aa`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184278f82293893eabe0e0cba0bb7778e131c4266f5344a1e8838252bab102a4`  
		Last Modified: Mon, 06 Jul 2020 20:55:10 GMT  
		Size: 138.8 MB (138808255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023eb94e085651a2a59ce390e764a8525f6384a8921216af5b5c422ed968c0b9`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4c175205f706c518b3f76fda81975f61062bb4768384e77161c31bb573663`  
		Last Modified: Mon, 06 Jul 2020 20:54:52 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:109b4ab288adc65d76ce96e55b95f29fb0bbec55c94cc7229467011af2bce0e8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6147207021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17259ef535401aa2eecc5f71db8414001c57dd82218715ba4c640ce91e4115ba`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:35:02 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:35:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:35:04 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 19:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 19:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 19:53:31 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 19:53:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54ffbdaf3aadb6b317220cf4e92b11a6de1c5cb2cc18dfa65f0f74174289503`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850856c450c610fe936d4092b2601b2e51954d4c2911765fdcbacd35c9265e16`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d696a21e0be15b220b32f5f1573e4f255971a8f4a4c4b5058a3ab7c9a82b24d`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa1aa83d1aa5af76b31fc1e8d919c8630b9bdd3c8c985537a2d55d4e99632b`  
		Last Modified: Mon, 06 Jul 2020 20:14:32 GMT  
		Size: 413.2 MB (413201285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1110553f1f1924f90747aaa9041b000ae8821e1e66550514c67d3430e3911`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42d6bf1851c5d28ec6834c663101351f365a3a3a86169e31f91931f0233a853`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882c76b8dbdc7c09c1cfcf05d32aef3a22187b433540e1c1b6c46c2cafd669f5`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:45501c1c91bba37313926453272963f0d30585198e51f206fb47232f2f6587f9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706281586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed675ff78b678261819c48b8150aa58c2ed7438c3a1ddeea86f74a43d92a71be`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:53:51 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 20:12:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 20:12:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 20:12:44 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:12:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4105bf49a3822f93914d7ee327ff44c4ac6bd3debfc2f5a7e2503b0c74a115e9`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d4c23eb9a1980b7fa0e2c063608e605f66c02f5459d3a216f1efff25311756`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0ef9898a4f3618d2308567c35f45b4627d2f17ba5d3c962442ae03811db38`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439fc0f14bbfa308c62b45b50deafd6ee77a4c70b040578048ea39ad6561c507`  
		Last Modified: Mon, 06 Jul 2020 20:15:37 GMT  
		Size: 412.4 MB (412359286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178148d52549bf2f86d42b2bed2cccc94c868f503202cb9e8353edae309d85`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7515e1d305d903836d5c895f3e180ffd54f905c0e09a9dbad3af32115451ea6`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e156991efd8447da6e3f368487d5c61184e32995f0db909e0a3b3ba82d59a10`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc-bionic`

```console
$ docker pull mongo@sha256:5e6a482a21dd96e46bf12a9a43e35141164df8c99d6749ffe66a79dc4c0d4c47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-rc-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:1f3d3a5056996ee2d79903b8b4bff07282c0509aa583ee5252808f360254eaaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177734791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8d7e328853dd0862396362278bf2dd5eef370d694d03207a18f66204eed5a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:04:01 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 22:04:03 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:04:03 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:04:03 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:04:03 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:04:03 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 22:04:04 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 22:04:04 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:04:24 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:04:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:04:28 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:04:28 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:04:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:04:28 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:04:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d37d7cdfd1b41d0e0691ef4fb5a6bfa57c3c93586e8f8ad0d1e2a0c30ef33e4`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 6.3 KB (6255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d870a78a337f4bf08d119f39dca63af37bc4a1be41c2c4e490c0a963c7c0d`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3fa6e90749b168660473aa9bb87538b7fe87ecb329dc7f074b4155d8086499`  
		Last Modified: Mon, 06 Jul 2020 22:06:20 GMT  
		Size: 142.2 MB (142192184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26368085ec6f36f53f5752930c4fca8f2f55ff73488f987b05eb9dd7a4acf2dc`  
		Last Modified: Mon, 06 Jul 2020 22:05:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f7e1b5994ab1fd1681edcbd0c5b1fdad271c456a9b6aee21a46509c9feef7`  
		Last Modified: Mon, 06 Jul 2020 22:05:57 GMT  
		Size: 4.0 KB (3957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:d3cd6c066a6fd832500419862eb08ae7177239461bca46014901928156820139
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167718774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e57fa87b22dfb173515f25b7d36041fe6ef590d96574866680370cc4c1c9a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:28:31 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 17 Jun 2020 03:28:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:28:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:28:39 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:28:41 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:28:42 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 20:41:41 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 20:41:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:42:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:42:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:42:45 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:42:46 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:42:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:42:47 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:42:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc22fb839309e0ff73d69148b1061567442476c00078e55fd8f2ca6fcd5c8`  
		Last Modified: Wed, 17 Jun 2020 03:31:47 GMT  
		Size: 6.3 KB (6253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f8978327ffb136a6c269d5dc77747e3ab023c8a6cc764d4245fe7c1e2bda67`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45f3afbd4755ff77072e256f3060cce5a18e8706317174784a0083750fe457e`  
		Last Modified: Mon, 06 Jul 2020 20:43:46 GMT  
		Size: 135.9 MB (135936675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1fb738b456ff8d587a791b61a9073840179d4ad43770e884614136adf99b6`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98555d93433808e042bcfd2219f52db76f2490128dfcfd100bfa8bb413544fc4`  
		Last Modified: Mon, 06 Jul 2020 20:43:15 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:46cd7bdac9a40b262a4551500c55506e432ab34ae10451c44ff0f43128bd3371
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172676863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f23234b61f437d2deff35ba0c81dc29750e02b2e053a8e3767e79ef1fd5156`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:38 GMT
ENV GPG_KEYS=99DC630F00A2F97F27C6A02A253612A09571B484 20691EEC35216C63CAF66CE1656408E390CFB1F5 E162F504A20CDF15827F718D4B7C549A058F8B6B 9DA31620334BD75D9DCB49F368818C72E52529D4 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 06 Jul 2020 20:53:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:40 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_MAJOR=testing
# Mon, 06 Jul 2020 20:53:40 GMT
ENV MONGO_VERSION=4.4.0~rc12
# Mon, 06 Jul 2020 20:53:41 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:54:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:54:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:54:06 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:54:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:54:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:54:06 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:54:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229cebbae25aab3e43b584e93b8164ce11270d4da12ef2f9982e34611a230f7c`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 6.3 KB (6256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5db194c8396d25a2f24c8f76f3dceff885a445d711e2f988022f89243776aa`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184278f82293893eabe0e0cba0bb7778e131c4266f5344a1e8838252bab102a4`  
		Last Modified: Mon, 06 Jul 2020 20:55:10 GMT  
		Size: 138.8 MB (138808255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023eb94e085651a2a59ce390e764a8525f6384a8921216af5b5c422ed968c0b9`  
		Last Modified: Mon, 06 Jul 2020 20:54:47 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4c175205f706c518b3f76fda81975f61062bb4768384e77161c31bb573663`  
		Last Modified: Mon, 06 Jul 2020 20:54:52 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc-windowsservercore`

```console
$ docker pull mongo@sha256:a06cac34470ae48d4542150fa06503a6f417781abb05d8aff635178bcee04361
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.4-rc-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:109b4ab288adc65d76ce96e55b95f29fb0bbec55c94cc7229467011af2bce0e8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6147207021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17259ef535401aa2eecc5f71db8414001c57dd82218715ba4c640ce91e4115ba`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:35:02 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:35:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:35:04 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 19:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 19:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 19:53:31 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 19:53:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54ffbdaf3aadb6b317220cf4e92b11a6de1c5cb2cc18dfa65f0f74174289503`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850856c450c610fe936d4092b2601b2e51954d4c2911765fdcbacd35c9265e16`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d696a21e0be15b220b32f5f1573e4f255971a8f4a4c4b5058a3ab7c9a82b24d`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa1aa83d1aa5af76b31fc1e8d919c8630b9bdd3c8c985537a2d55d4e99632b`  
		Last Modified: Mon, 06 Jul 2020 20:14:32 GMT  
		Size: 413.2 MB (413201285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1110553f1f1924f90747aaa9041b000ae8821e1e66550514c67d3430e3911`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42d6bf1851c5d28ec6834c663101351f365a3a3a86169e31f91931f0233a853`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882c76b8dbdc7c09c1cfcf05d32aef3a22187b433540e1c1b6c46c2cafd669f5`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-rc-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:45501c1c91bba37313926453272963f0d30585198e51f206fb47232f2f6587f9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706281586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed675ff78b678261819c48b8150aa58c2ed7438c3a1ddeea86f74a43d92a71be`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:53:51 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 20:12:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 20:12:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 20:12:44 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:12:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4105bf49a3822f93914d7ee327ff44c4ac6bd3debfc2f5a7e2503b0c74a115e9`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d4c23eb9a1980b7fa0e2c063608e605f66c02f5459d3a216f1efff25311756`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0ef9898a4f3618d2308567c35f45b4627d2f17ba5d3c962442ae03811db38`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439fc0f14bbfa308c62b45b50deafd6ee77a4c70b040578048ea39ad6561c507`  
		Last Modified: Mon, 06 Jul 2020 20:15:37 GMT  
		Size: 412.4 MB (412359286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178148d52549bf2f86d42b2bed2cccc94c868f503202cb9e8353edae309d85`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7515e1d305d903836d5c895f3e180ffd54f905c0e09a9dbad3af32115451ea6`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e156991efd8447da6e3f368487d5c61184e32995f0db909e0a3b3ba82d59a10`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc-windowsservercore-1809`

```console
$ docker pull mongo@sha256:94224515f3dd271bfa26f9ce7b0c3037842376ed3d7c4b4939dcd8dcb127cda4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:4.4-rc-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:45501c1c91bba37313926453272963f0d30585198e51f206fb47232f2f6587f9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706281586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed675ff78b678261819c48b8150aa58c2ed7438c3a1ddeea86f74a43d92a71be`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:53:51 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:53:52 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 20:12:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 20:12:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 20:12:44 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:12:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4105bf49a3822f93914d7ee327ff44c4ac6bd3debfc2f5a7e2503b0c74a115e9`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d4c23eb9a1980b7fa0e2c063608e605f66c02f5459d3a216f1efff25311756`  
		Last Modified: Mon, 06 Jul 2020 20:14:44 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0ef9898a4f3618d2308567c35f45b4627d2f17ba5d3c962442ae03811db38`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439fc0f14bbfa308c62b45b50deafd6ee77a4c70b040578048ea39ad6561c507`  
		Last Modified: Mon, 06 Jul 2020 20:15:37 GMT  
		Size: 412.4 MB (412359286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178148d52549bf2f86d42b2bed2cccc94c868f503202cb9e8353edae309d85`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7515e1d305d903836d5c895f3e180ffd54f905c0e09a9dbad3af32115451ea6`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e156991efd8447da6e3f368487d5c61184e32995f0db909e0a3b3ba82d59a10`  
		Last Modified: Mon, 06 Jul 2020 20:14:42 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-rc-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:b1ba9f21ebd21d2627f9a72b1bd16263ba9f3940994a4ccfe05b2be1c6c3d4fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:4.4-rc-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:109b4ab288adc65d76ce96e55b95f29fb0bbec55c94cc7229467011af2bce0e8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6147207021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17259ef535401aa2eecc5f71db8414001c57dd82218715ba4c640ce91e4115ba`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 06 Jul 2020 19:35:02 GMT
ENV MONGO_VERSION=4.4.0-rc12
# Mon, 06 Jul 2020 19:35:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-rc12-signed.msi
# Mon, 06 Jul 2020 19:35:04 GMT
ENV MONGO_DOWNLOAD_SHA256=878808010793c330f1c1e0f73b917e4a48c2484cef8f727848a99dd387cce3da
# Mon, 06 Jul 2020 19:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 06 Jul 2020 19:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 06 Jul 2020 19:53:31 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 19:53:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54ffbdaf3aadb6b317220cf4e92b11a6de1c5cb2cc18dfa65f0f74174289503`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850856c450c610fe936d4092b2601b2e51954d4c2911765fdcbacd35c9265e16`  
		Last Modified: Mon, 06 Jul 2020 20:13:47 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d696a21e0be15b220b32f5f1573e4f255971a8f4a4c4b5058a3ab7c9a82b24d`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa1aa83d1aa5af76b31fc1e8d919c8630b9bdd3c8c985537a2d55d4e99632b`  
		Last Modified: Mon, 06 Jul 2020 20:14:32 GMT  
		Size: 413.2 MB (413201285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1110553f1f1924f90747aaa9041b000ae8821e1e66550514c67d3430e3911`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42d6bf1851c5d28ec6834c663101351f365a3a3a86169e31f91931f0233a853`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882c76b8dbdc7c09c1cfcf05d32aef3a22187b433540e1c1b6c46c2cafd669f5`  
		Last Modified: Mon, 06 Jul 2020 20:13:44 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:27721e00fde059507056a18d6b699ea3965941933ac2d01820ebdfaa88460f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:94c26811b76f697fa9ed91431d3665cfc6d87254c7980ddf2510c55833700835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164659719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d11486a97a77beaad31f63463a744dc3070ed4070bd15a695898a171f349441`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:03:34 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 22:03:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:03:35 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:03:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 22:03:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:03:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:03:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:03:56 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:03:56 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:03:57 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b916e924f1778f3230a1b137a675f2e8be7000c8c85e63e1c6432bcaaf12b5`  
		Last Modified: Mon, 06 Jul 2020 22:05:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805b21b6014c2d2a6a6ec4196c020291a87385046ae71c50dbb266113315e17`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7775fed6386269ff74f698e1b016ac356ee5f2299e86d2ab1ab4f09456fe2735`  
		Last Modified: Mon, 06 Jul 2020 22:05:52 GMT  
		Size: 129.1 MB (129121934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94226c388074f114ce594ea4a972fbead3f892e931da7b6918393f5994be1778`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7bf6a32e97cd93a1351b98c52cc7518f0d0592b48ee15aa03d2dc08d42653`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cdec0bd28e60bc06892f9972803753d57fdc3d4bcff657b694ba7f35b80d3d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154677642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84af28ce3aa3b7b04964d7f7ee9eb0ae10e3c19e684ad29ceeca55c605f2924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:27:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 17 Jun 2020 03:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:27:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:27:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:19 GMT
ENV MONGO_MAJOR=4.2
# Wed, 17 Jun 2020 03:27:20 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 03:27:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:28:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:28:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:28:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:28:08 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:28:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2b58fe1082de604f779b26f7bac0f685326b5584f5a43457f1d51effdca86`  
		Last Modified: Wed, 17 Jun 2020 03:31:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52cb618aa3e851b5a35792b706fd4e70901c2e3fd1faa3fcf12d719ac3d8ff1`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8985f89f29dd85eccbd8da50a080817fa846f7b7baee89e54e83f79559fff4b`  
		Last Modified: Wed, 17 Jun 2020 03:31:35 GMT  
		Size: 122.9 MB (122900361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f01ca57315b3f1a9469f85034d0f072b2d67b5ee9d3c9d2e14e3487df4db4d`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414fc1b8d9a096289a531b03096d4af7478a1c627842175a15974cb041c879`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:fd127fabc1bf86887613c1468da9458cdc40911ecb2be77512c0eff1abab7fad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160601784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8f620c8146e13765df833a4b47d557436a720571e885a22723c1431b1e0692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 20:53:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 20:53:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:53:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:53:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:53:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:53:32 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:53:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:53:33 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:53:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58902fb585e4821ffa80bd89abeaa891bf6f300ea302d85c089768fb721eacc`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51829b8cf8dd38c72c0f94d87ff4af39d009f29247ca7c0e56ad482bf229f4e`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afc8f2fd906dff6030983b0b511c3de126fcdf5255f7a6f1682b4a6e97fd3a`  
		Last Modified: Mon, 06 Jul 2020 20:54:39 GMT  
		Size: 126.7 MB (126738005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1641f60d50a5f6029e584a560748712b711521aa9d0c1c87e91ef2a4cb32ea8c`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6c42abe7efd4b6acc1c8ce6b0aac98da4da44252eb5710466004737e77342`  
		Last Modified: Mon, 06 Jul 2020 20:54:40 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:3dfacb1c248e30392bcfaba258677f7a057a4ea96b2a37de4839a01081742a64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:4-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:bc2bc28a30754135707bfc25dd73c4aceb4ae89c943a243433b0b3f321f640fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b6e497bdcaa3a451d4296f944c0a13ac07344a7879cb41fb387ae288308fc61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:27721e00fde059507056a18d6b699ea3965941933ac2d01820ebdfaa88460f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:94c26811b76f697fa9ed91431d3665cfc6d87254c7980ddf2510c55833700835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164659719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d11486a97a77beaad31f63463a744dc3070ed4070bd15a695898a171f349441`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:03:34 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 22:03:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:03:35 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:03:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 22:03:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:03:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:03:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:03:56 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:03:56 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:03:57 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b916e924f1778f3230a1b137a675f2e8be7000c8c85e63e1c6432bcaaf12b5`  
		Last Modified: Mon, 06 Jul 2020 22:05:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805b21b6014c2d2a6a6ec4196c020291a87385046ae71c50dbb266113315e17`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7775fed6386269ff74f698e1b016ac356ee5f2299e86d2ab1ab4f09456fe2735`  
		Last Modified: Mon, 06 Jul 2020 22:05:52 GMT  
		Size: 129.1 MB (129121934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94226c388074f114ce594ea4a972fbead3f892e931da7b6918393f5994be1778`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7bf6a32e97cd93a1351b98c52cc7518f0d0592b48ee15aa03d2dc08d42653`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cdec0bd28e60bc06892f9972803753d57fdc3d4bcff657b694ba7f35b80d3d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154677642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84af28ce3aa3b7b04964d7f7ee9eb0ae10e3c19e684ad29ceeca55c605f2924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:27:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 17 Jun 2020 03:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:27:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:27:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:19 GMT
ENV MONGO_MAJOR=4.2
# Wed, 17 Jun 2020 03:27:20 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 03:27:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:28:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:28:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:28:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:28:08 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:28:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2b58fe1082de604f779b26f7bac0f685326b5584f5a43457f1d51effdca86`  
		Last Modified: Wed, 17 Jun 2020 03:31:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52cb618aa3e851b5a35792b706fd4e70901c2e3fd1faa3fcf12d719ac3d8ff1`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8985f89f29dd85eccbd8da50a080817fa846f7b7baee89e54e83f79559fff4b`  
		Last Modified: Wed, 17 Jun 2020 03:31:35 GMT  
		Size: 122.9 MB (122900361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f01ca57315b3f1a9469f85034d0f072b2d67b5ee9d3c9d2e14e3487df4db4d`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414fc1b8d9a096289a531b03096d4af7478a1c627842175a15974cb041c879`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:fd127fabc1bf86887613c1468da9458cdc40911ecb2be77512c0eff1abab7fad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160601784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8f620c8146e13765df833a4b47d557436a720571e885a22723c1431b1e0692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 20:53:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 20:53:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:53:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:53:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:53:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:53:32 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:53:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:53:33 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:53:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58902fb585e4821ffa80bd89abeaa891bf6f300ea302d85c089768fb721eacc`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51829b8cf8dd38c72c0f94d87ff4af39d009f29247ca7c0e56ad482bf229f4e`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afc8f2fd906dff6030983b0b511c3de126fcdf5255f7a6f1682b4a6e97fd3a`  
		Last Modified: Mon, 06 Jul 2020 20:54:39 GMT  
		Size: 126.7 MB (126738005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1641f60d50a5f6029e584a560748712b711521aa9d0c1c87e91ef2a4cb32ea8c`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6c42abe7efd4b6acc1c8ce6b0aac98da4da44252eb5710466004737e77342`  
		Last Modified: Mon, 06 Jul 2020 20:54:40 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:37047f9762ca311dc2c84883c199b984322b82fc38097ac39624a8b98b15884d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:94c26811b76f697fa9ed91431d3665cfc6d87254c7980ddf2510c55833700835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164659719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d11486a97a77beaad31f63463a744dc3070ed4070bd15a695898a171f349441`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:03:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 22:03:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:03:17 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 22:03:17 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 22:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 22:03:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 22:03:34 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 22:03:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 22:03:35 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 22:03:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 22:03:36 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 22:03:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 22:03:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 22:03:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 22:03:56 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 22:03:56 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 22:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 22:03:57 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 22:03:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af850482677968f32d51ae4d2c60321c548d8c7abc4f55a9ee759c21a5d59586`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faaabd5f8b25c4747d46f9ac3b1652b014176d3d4f1b9c0e1061c6031f190f0`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 3.0 MB (2973549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bb90b3c1e5e84d9ccc830058d9b5f597b75fd22d9e6f76200195ab771b3c89`  
		Last Modified: Mon, 06 Jul 2020 22:05:35 GMT  
		Size: 5.8 MB (5823906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f4b579cf84af9882529d5fc3c5a66447299886f687b0e6cd12e621cdde4eda`  
		Last Modified: Mon, 06 Jul 2020 22:05:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b916e924f1778f3230a1b137a675f2e8be7000c8c85e63e1c6432bcaaf12b5`  
		Last Modified: Mon, 06 Jul 2020 22:05:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805b21b6014c2d2a6a6ec4196c020291a87385046ae71c50dbb266113315e17`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7775fed6386269ff74f698e1b016ac356ee5f2299e86d2ab1ab4f09456fe2735`  
		Last Modified: Mon, 06 Jul 2020 22:05:52 GMT  
		Size: 129.1 MB (129121934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94226c388074f114ce594ea4a972fbead3f892e931da7b6918393f5994be1778`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf7bf6a32e97cd93a1351b98c52cc7518f0d0592b48ee15aa03d2dc08d42653`  
		Last Modified: Mon, 06 Jul 2020 22:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cdec0bd28e60bc06892f9972803753d57fdc3d4bcff657b694ba7f35b80d3d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154677642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84af28ce3aa3b7b04964d7f7ee9eb0ae10e3c19e684ad29ceeca55c605f2924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:26:00 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 17 Jun 2020 03:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:26:24 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Jun 2020 03:26:25 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 17 Jun 2020 03:27:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Jun 2020 03:27:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jun 2020 03:27:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 17 Jun 2020 03:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jun 2020 03:27:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 17 Jun 2020 03:27:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:16 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 17 Jun 2020 03:27:19 GMT
ENV MONGO_MAJOR=4.2
# Wed, 17 Jun 2020 03:27:20 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 03:27:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jun 2020 03:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jun 2020 03:28:02 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jun 2020 03:28:04 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jun 2020 03:28:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 17 Jun 2020 03:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:28:08 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 03:28:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f4068e2fc9c5ce913c3640637c35584b72816ca9485c4bf5af0a22994d0f6`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5678c55b212ca2ce4ea7b4092838653b706277000f57d7a18526f3df6cba283`  
		Last Modified: Wed, 17 Jun 2020 03:31:11 GMT  
		Size: 2.7 MB (2665976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509de0ccfb79a34de230a6fef2cfc900bdb35f1f7f583fc957b7c23b46439d4f`  
		Last Modified: Wed, 17 Jun 2020 03:31:12 GMT  
		Size: 5.3 MB (5345550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5493b54160873a149e08eedf09e74628680b1d5e8826b90672f04c88c30ccb`  
		Last Modified: Wed, 17 Jun 2020 03:31:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2b58fe1082de604f779b26f7bac0f685326b5584f5a43457f1d51effdca86`  
		Last Modified: Wed, 17 Jun 2020 03:31:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52cb618aa3e851b5a35792b706fd4e70901c2e3fd1faa3fcf12d719ac3d8ff1`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8985f89f29dd85eccbd8da50a080817fa846f7b7baee89e54e83f79559fff4b`  
		Last Modified: Wed, 17 Jun 2020 03:31:35 GMT  
		Size: 122.9 MB (122900361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f01ca57315b3f1a9469f85034d0f072b2d67b5ee9d3c9d2e14e3487df4db4d`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414fc1b8d9a096289a531b03096d4af7478a1c627842175a15974cb041c879`  
		Last Modified: Wed, 17 Jun 2020 03:31:08 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:fd127fabc1bf86887613c1468da9458cdc40911ecb2be77512c0eff1abab7fad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160601784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8f620c8146e13765df833a4b47d557436a720571e885a22723c1431b1e0692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:52:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 06 Jul 2020 20:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:52:58 GMT
ENV GOSU_VERSION=1.12
# Mon, 06 Jul 2020 20:52:58 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 06 Jul 2020 20:53:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 06 Jul 2020 20:53:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 06 Jul 2020 20:53:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 06 Jul 2020 20:53:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 06 Jul 2020 20:53:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_MAJOR=4.2
# Mon, 06 Jul 2020 20:53:12 GMT
ENV MONGO_VERSION=4.2.8
# Mon, 06 Jul 2020 20:53:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 06 Jul 2020 20:53:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 06 Jul 2020 20:53:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 06 Jul 2020 20:53:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 06 Jul 2020 20:53:32 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 06 Jul 2020 20:53:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jul 2020 20:53:33 GMT
EXPOSE 27017
# Mon, 06 Jul 2020 20:53:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d54d163a3f780399465ae6c4d8e5c12835af02ce8c7b73e5f1a15fbc21c50`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4800ea211f8b53f2ef80acbdd85aee0a999ec837ce72cb976aa99d215deefaa7`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 2.7 MB (2704448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664da75ca96edb5c84ed38526be8fc2f6fb1c4455d2403762b2678a91cb9c86b`  
		Last Modified: Mon, 06 Jul 2020 20:54:27 GMT  
		Size: 5.7 MB (5745092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e65e9a2011b91ec44b9c2b893eeec832eddad99a284ca930a4bf0cc8b3eb02`  
		Last Modified: Mon, 06 Jul 2020 20:54:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58902fb585e4821ffa80bd89abeaa891bf6f300ea302d85c089768fb721eacc`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51829b8cf8dd38c72c0f94d87ff4af39d009f29247ca7c0e56ad482bf229f4e`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afc8f2fd906dff6030983b0b511c3de126fcdf5255f7a6f1682b4a6e97fd3a`  
		Last Modified: Mon, 06 Jul 2020 20:54:39 GMT  
		Size: 126.7 MB (126738005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1641f60d50a5f6029e584a560748712b711521aa9d0c1c87e91ef2a4cb32ea8c`  
		Last Modified: Mon, 06 Jul 2020 20:54:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6c42abe7efd4b6acc1c8ce6b0aac98da4da44252eb5710466004737e77342`  
		Last Modified: Mon, 06 Jul 2020 20:54:40 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:3dfacb1c248e30392bcfaba258677f7a057a4ea96b2a37de4839a01081742a64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:bc2bc28a30754135707bfc25dd73c4aceb4ae89c943a243433b0b3f321f640fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:a332d0d55bcb861ab664609d4ee8b7a3c7481e800fa5ad62009c671c1673af0b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752054828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86c12ab59b3d8850d880c02f06724769d7955a42bb4c5b10fd9a16cb6ad19f7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 01:09:02 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 01:09:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 01:09:04 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:28:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:28:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:28:18 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:28:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51df57f2cb6ccc03b57cbd044ee4a49d9383489feb3872da465ba8b6bffa89`  
		Last Modified: Wed, 17 Jun 2020 01:33:19 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84353c49610a99480bfb74a8769e7446bbd898b8644c25d2b8c645c7a2e90e0e`  
		Last Modified: Wed, 17 Jun 2020 01:33:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c19d206596ed0cd1b7da30ba6e637be1d4c31dc398ca6f4d30d583593e31705`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90fa0f2b93199d15d0678aa8a13db7d1470a5ce7ddb94ec8fa93a75156cce44`  
		Last Modified: Wed, 17 Jun 2020 01:34:14 GMT  
		Size: 458.1 MB (458132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369180762b76f75c56ed85ad59e938011c514ad32b51a43cbb6d5fcce885b5d1`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f9c110c11f811446f2204714562c02b6eefeeb1cae671aa73af5e4cc7dfbd0`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7a275e52c9eafb08caf7a861ef21a725b77ee54c1b867ddb4b4da99814dd7`  
		Last Modified: Wed, 17 Jun 2020 01:33:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b6e497bdcaa3a451d4296f944c0a13ac07344a7879cb41fb387ae288308fc61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:af38590235375eb1218ddd651e660f1a6e6e6a882842e7b428f2d55d46cc937a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6193023222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaf2b53fe9e096da5ab6f4ae0e34caf7cf3de0a336bd9576cee60752c37c17b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 17 Jun 2020 00:50:43 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 17 Jun 2020 00:50:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 17 Jun 2020 00:50:45 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 17 Jun 2020 01:08:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 17 Jun 2020 01:08:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 17 Jun 2020 01:08:53 GMT
EXPOSE 27017
# Wed, 17 Jun 2020 01:08:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b60479ef88c8a931aeeffaa74d289fbbf204229adb6a20c54d51456f70bb75`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bb592e6eb6512ccf1127b0311263697d559599357972414f4b776277bd628f`  
		Last Modified: Wed, 17 Jun 2020 01:32:04 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b55cda98f10b8c536232f9fd5fbc19c778c4043edc4fea012972832bb4570`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaad7a52f6dc4a311c3e724f9b5fe27f7af849fa6229fe21fc0490976fcb607`  
		Last Modified: Wed, 17 Jun 2020 01:32:57 GMT  
		Size: 459.0 MB (459017760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187b8e518ef05e3f4e7348e0ca7fef3e05414c63661223d63d83a36367ff9605`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58773855217e4f81876fd21fd13a61d94d0f5a191e7025ce2bf26469077e330c`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f1762a4dcad6fd6709c2602e0d459a0efb6aea6e10e16cb78796c27e496d`  
		Last Modified: Wed, 17 Jun 2020 01:32:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
