<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.17`](#mongo3617)
-	[`mongo:3.6.17-windowsservercore`](#mongo3617-windowsservercore)
-	[`mongo:3.6.17-windowsservercore-1809`](#mongo3617-windowsservercore-1809)
-	[`mongo:3.6.17-windowsservercore-ltsc2016`](#mongo3617-windowsservercore-ltsc2016)
-	[`mongo:3.6.17-xenial`](#mongo3617-xenial)
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
-	[`mongo:4.0.17`](#mongo4017)
-	[`mongo:4.0.17-windowsservercore`](#mongo4017-windowsservercore)
-	[`mongo:4.0.17-windowsservercore-1809`](#mongo4017-windowsservercore-1809)
-	[`mongo:4.0.17-windowsservercore-ltsc2016`](#mongo4017-windowsservercore-ltsc2016)
-	[`mongo:4.0.17-xenial`](#mongo4017-xenial)
-	[`mongo:4.0-windowsservercore`](#mongo40-windowsservercore)
-	[`mongo:4.0-windowsservercore-1809`](#mongo40-windowsservercore-1809)
-	[`mongo:4.0-windowsservercore-ltsc2016`](#mongo40-windowsservercore-ltsc2016)
-	[`mongo:4.0-xenial`](#mongo40-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2.5`](#mongo425)
-	[`mongo:4.2.5-bionic`](#mongo425-bionic)
-	[`mongo:4.2.5-windowsservercore`](#mongo425-windowsservercore)
-	[`mongo:4.2.5-windowsservercore-1809`](#mongo425-windowsservercore-1809)
-	[`mongo:4.2.5-windowsservercore-ltsc2016`](#mongo425-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:7ca7e3b6a76643ad168b0e16b78cd6e5a018db6596671ee1571505ae6f630dcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:557aaf306c611bf9cd04e69fc3174757e2ce25ecc073a88fe28dbc889f5dae9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165644020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fdbdf0f17b70466eda08d155b2f1c72bc3450d23b8a752a4a841a83d6eb76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:08:41 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 22 Feb 2020 01:08:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_MAJOR=3.6
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_VERSION=3.6.17
# Sat, 22 Feb 2020 01:08:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 22 Feb 2020 01:09:04 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 22 Feb 2020 01:09:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 22 Feb 2020 01:09:05 GMT
VOLUME [/data/db /data/configdb]
# Sat, 22 Feb 2020 01:09:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 22 Feb 2020 01:09:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 01:09:06 GMT
EXPOSE 27017
# Sat, 22 Feb 2020 01:09:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03380f32ca06a89bb8bbb6437140f7feaa8cbc73656efd413066485af7bed9`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a38c136f14bc4cc8e7c8b75a1b58fbd13ee66ab4018835cce5deafd77e34629`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0e875b59ceec4323d6455ddef1a97e267ed64e723a3785961db869da21e662`  
		Last Modified: Sat, 22 Feb 2020 01:11:19 GMT  
		Size: 117.3 MB (117252414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f55b4999cd606166300c3bcc0c29bbdb69f9e442f652f9e2a1b037ff63069d`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc92ef8de8b080701461ef5a44e3df6e2b20f0e5d0502bc9c2f58fb0c18884c`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8d00f2129c233839b0192bc63ad1b38d732559eb063a8c7fb6afd9b14000dfe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155054951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904d1cc8fa66fbab1604f0f278d0125cf824c48dde0e06e2de53f80f21123a3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:48:51 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 21 Feb 2020 22:48:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:56 GMT
ENV MONGO_MAJOR=3.6
# Fri, 21 Feb 2020 22:48:57 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 21 Feb 2020 22:48:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 21 Feb 2020 22:49:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 21 Feb 2020 22:49:23 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 21 Feb 2020 22:49:24 GMT
VOLUME [/data/db /data/configdb]
# Fri, 21 Feb 2020 22:49:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 21 Feb 2020 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 22:49:26 GMT
EXPOSE 27017
# Fri, 21 Feb 2020 22:49:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c551726d412935a665a5faa37ba35c6b578c9b4b9a04e15fbb8141e18c469f4`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690416c5e0de4a88eb11a3f888d668dffc71c64ce9928810382a5f989ea0d6d8`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466edf90a60ac36b2e4ef9846aac45cf6dcbf6603561ff365607d6ec8e1d4333`  
		Last Modified: Fri, 21 Feb 2020 22:53:01 GMT  
		Size: 111.5 MB (111459661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a78ae9c5bd995e33cabe28ea21119ec5a46c4ecd1c7a5b80beedf81e226048`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfad788e158cc0e6900c305454fae286feb8c8e9807a24c9e4a962a22727dfc`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:7ca7e3b6a76643ad168b0e16b78cd6e5a018db6596671ee1571505ae6f630dcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:557aaf306c611bf9cd04e69fc3174757e2ce25ecc073a88fe28dbc889f5dae9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165644020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fdbdf0f17b70466eda08d155b2f1c72bc3450d23b8a752a4a841a83d6eb76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:08:41 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 22 Feb 2020 01:08:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_MAJOR=3.6
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_VERSION=3.6.17
# Sat, 22 Feb 2020 01:08:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 22 Feb 2020 01:09:04 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 22 Feb 2020 01:09:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 22 Feb 2020 01:09:05 GMT
VOLUME [/data/db /data/configdb]
# Sat, 22 Feb 2020 01:09:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 22 Feb 2020 01:09:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 01:09:06 GMT
EXPOSE 27017
# Sat, 22 Feb 2020 01:09:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03380f32ca06a89bb8bbb6437140f7feaa8cbc73656efd413066485af7bed9`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a38c136f14bc4cc8e7c8b75a1b58fbd13ee66ab4018835cce5deafd77e34629`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0e875b59ceec4323d6455ddef1a97e267ed64e723a3785961db869da21e662`  
		Last Modified: Sat, 22 Feb 2020 01:11:19 GMT  
		Size: 117.3 MB (117252414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f55b4999cd606166300c3bcc0c29bbdb69f9e442f652f9e2a1b037ff63069d`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc92ef8de8b080701461ef5a44e3df6e2b20f0e5d0502bc9c2f58fb0c18884c`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8d00f2129c233839b0192bc63ad1b38d732559eb063a8c7fb6afd9b14000dfe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155054951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904d1cc8fa66fbab1604f0f278d0125cf824c48dde0e06e2de53f80f21123a3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:48:51 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 21 Feb 2020 22:48:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:56 GMT
ENV MONGO_MAJOR=3.6
# Fri, 21 Feb 2020 22:48:57 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 21 Feb 2020 22:48:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 21 Feb 2020 22:49:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 21 Feb 2020 22:49:23 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 21 Feb 2020 22:49:24 GMT
VOLUME [/data/db /data/configdb]
# Fri, 21 Feb 2020 22:49:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 21 Feb 2020 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 22:49:26 GMT
EXPOSE 27017
# Fri, 21 Feb 2020 22:49:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c551726d412935a665a5faa37ba35c6b578c9b4b9a04e15fbb8141e18c469f4`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690416c5e0de4a88eb11a3f888d668dffc71c64ce9928810382a5f989ea0d6d8`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466edf90a60ac36b2e4ef9846aac45cf6dcbf6603561ff365607d6ec8e1d4333`  
		Last Modified: Fri, 21 Feb 2020 22:53:01 GMT  
		Size: 111.5 MB (111459661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a78ae9c5bd995e33cabe28ea21119ec5a46c4ecd1c7a5b80beedf81e226048`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfad788e158cc0e6900c305454fae286feb8c8e9807a24c9e4a962a22727dfc`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17`

```console
$ docker pull mongo@sha256:7ca7e3b6a76643ad168b0e16b78cd6e5a018db6596671ee1571505ae6f630dcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:3.6.17` - linux; amd64

```console
$ docker pull mongo@sha256:557aaf306c611bf9cd04e69fc3174757e2ce25ecc073a88fe28dbc889f5dae9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165644020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fdbdf0f17b70466eda08d155b2f1c72bc3450d23b8a752a4a841a83d6eb76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:08:41 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 22 Feb 2020 01:08:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_MAJOR=3.6
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_VERSION=3.6.17
# Sat, 22 Feb 2020 01:08:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 22 Feb 2020 01:09:04 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 22 Feb 2020 01:09:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 22 Feb 2020 01:09:05 GMT
VOLUME [/data/db /data/configdb]
# Sat, 22 Feb 2020 01:09:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 22 Feb 2020 01:09:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 01:09:06 GMT
EXPOSE 27017
# Sat, 22 Feb 2020 01:09:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03380f32ca06a89bb8bbb6437140f7feaa8cbc73656efd413066485af7bed9`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a38c136f14bc4cc8e7c8b75a1b58fbd13ee66ab4018835cce5deafd77e34629`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0e875b59ceec4323d6455ddef1a97e267ed64e723a3785961db869da21e662`  
		Last Modified: Sat, 22 Feb 2020 01:11:19 GMT  
		Size: 117.3 MB (117252414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f55b4999cd606166300c3bcc0c29bbdb69f9e442f652f9e2a1b037ff63069d`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc92ef8de8b080701461ef5a44e3df6e2b20f0e5d0502bc9c2f58fb0c18884c`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8d00f2129c233839b0192bc63ad1b38d732559eb063a8c7fb6afd9b14000dfe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155054951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904d1cc8fa66fbab1604f0f278d0125cf824c48dde0e06e2de53f80f21123a3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:48:51 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 21 Feb 2020 22:48:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:56 GMT
ENV MONGO_MAJOR=3.6
# Fri, 21 Feb 2020 22:48:57 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 21 Feb 2020 22:48:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 21 Feb 2020 22:49:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 21 Feb 2020 22:49:23 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 21 Feb 2020 22:49:24 GMT
VOLUME [/data/db /data/configdb]
# Fri, 21 Feb 2020 22:49:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 21 Feb 2020 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 22:49:26 GMT
EXPOSE 27017
# Fri, 21 Feb 2020 22:49:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c551726d412935a665a5faa37ba35c6b578c9b4b9a04e15fbb8141e18c469f4`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690416c5e0de4a88eb11a3f888d668dffc71c64ce9928810382a5f989ea0d6d8`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466edf90a60ac36b2e4ef9846aac45cf6dcbf6603561ff365607d6ec8e1d4333`  
		Last Modified: Fri, 21 Feb 2020 22:53:01 GMT  
		Size: 111.5 MB (111459661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a78ae9c5bd995e33cabe28ea21119ec5a46c4ecd1c7a5b80beedf81e226048`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfad788e158cc0e6900c305454fae286feb8c8e9807a24c9e4a962a22727dfc`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17-windowsservercore`

```console
$ docker pull mongo@sha256:0f92e13d622544ed93898c56cd2b7dc2a2cf69fcc9de3b796cc4c385bea87791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:3.6.17-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17-windowsservercore-1809`

```console
$ docker pull mongo@sha256:ba754b60411d37b3518e23450efea880bd623745c95513e1e7244b252451b24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:3.6.17-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:5b86c671b4e30d6934384b87e9e0e7ec2c1e1c995737c8f9cd64a59879627e1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:3.6.17-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17-xenial`

```console
$ docker pull mongo@sha256:dbdd944e50ed4f45174aae05205e284b76166e3ac9801b6f15856b79fb3f595b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.17-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:557aaf306c611bf9cd04e69fc3174757e2ce25ecc073a88fe28dbc889f5dae9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165644020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fdbdf0f17b70466eda08d155b2f1c72bc3450d23b8a752a4a841a83d6eb76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:08:41 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 22 Feb 2020 01:08:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_MAJOR=3.6
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_VERSION=3.6.17
# Sat, 22 Feb 2020 01:08:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 22 Feb 2020 01:09:04 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 22 Feb 2020 01:09:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 22 Feb 2020 01:09:05 GMT
VOLUME [/data/db /data/configdb]
# Sat, 22 Feb 2020 01:09:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 22 Feb 2020 01:09:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 01:09:06 GMT
EXPOSE 27017
# Sat, 22 Feb 2020 01:09:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03380f32ca06a89bb8bbb6437140f7feaa8cbc73656efd413066485af7bed9`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a38c136f14bc4cc8e7c8b75a1b58fbd13ee66ab4018835cce5deafd77e34629`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0e875b59ceec4323d6455ddef1a97e267ed64e723a3785961db869da21e662`  
		Last Modified: Sat, 22 Feb 2020 01:11:19 GMT  
		Size: 117.3 MB (117252414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f55b4999cd606166300c3bcc0c29bbdb69f9e442f652f9e2a1b037ff63069d`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc92ef8de8b080701461ef5a44e3df6e2b20f0e5d0502bc9c2f58fb0c18884c`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8d00f2129c233839b0192bc63ad1b38d732559eb063a8c7fb6afd9b14000dfe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155054951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904d1cc8fa66fbab1604f0f278d0125cf824c48dde0e06e2de53f80f21123a3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:48:51 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 21 Feb 2020 22:48:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:56 GMT
ENV MONGO_MAJOR=3.6
# Fri, 21 Feb 2020 22:48:57 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 21 Feb 2020 22:48:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 21 Feb 2020 22:49:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 21 Feb 2020 22:49:23 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 21 Feb 2020 22:49:24 GMT
VOLUME [/data/db /data/configdb]
# Fri, 21 Feb 2020 22:49:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 21 Feb 2020 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 22:49:26 GMT
EXPOSE 27017
# Fri, 21 Feb 2020 22:49:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c551726d412935a665a5faa37ba35c6b578c9b4b9a04e15fbb8141e18c469f4`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690416c5e0de4a88eb11a3f888d668dffc71c64ce9928810382a5f989ea0d6d8`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466edf90a60ac36b2e4ef9846aac45cf6dcbf6603561ff365607d6ec8e1d4333`  
		Last Modified: Fri, 21 Feb 2020 22:53:01 GMT  
		Size: 111.5 MB (111459661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a78ae9c5bd995e33cabe28ea21119ec5a46c4ecd1c7a5b80beedf81e226048`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfad788e158cc0e6900c305454fae286feb8c8e9807a24c9e4a962a22727dfc`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:0f92e13d622544ed93898c56cd2b7dc2a2cf69fcc9de3b796cc4c385bea87791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:ba754b60411d37b3518e23450efea880bd623745c95513e1e7244b252451b24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:5b86c671b4e30d6934384b87e9e0e7ec2c1e1c995737c8f9cd64a59879627e1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:dbdd944e50ed4f45174aae05205e284b76166e3ac9801b6f15856b79fb3f595b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:557aaf306c611bf9cd04e69fc3174757e2ce25ecc073a88fe28dbc889f5dae9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165644020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fdbdf0f17b70466eda08d155b2f1c72bc3450d23b8a752a4a841a83d6eb76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:08:41 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 22 Feb 2020 01:08:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_MAJOR=3.6
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_VERSION=3.6.17
# Sat, 22 Feb 2020 01:08:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 22 Feb 2020 01:09:04 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 22 Feb 2020 01:09:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 22 Feb 2020 01:09:05 GMT
VOLUME [/data/db /data/configdb]
# Sat, 22 Feb 2020 01:09:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 22 Feb 2020 01:09:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 01:09:06 GMT
EXPOSE 27017
# Sat, 22 Feb 2020 01:09:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03380f32ca06a89bb8bbb6437140f7feaa8cbc73656efd413066485af7bed9`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a38c136f14bc4cc8e7c8b75a1b58fbd13ee66ab4018835cce5deafd77e34629`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0e875b59ceec4323d6455ddef1a97e267ed64e723a3785961db869da21e662`  
		Last Modified: Sat, 22 Feb 2020 01:11:19 GMT  
		Size: 117.3 MB (117252414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f55b4999cd606166300c3bcc0c29bbdb69f9e442f652f9e2a1b037ff63069d`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc92ef8de8b080701461ef5a44e3df6e2b20f0e5d0502bc9c2f58fb0c18884c`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8d00f2129c233839b0192bc63ad1b38d732559eb063a8c7fb6afd9b14000dfe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155054951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904d1cc8fa66fbab1604f0f278d0125cf824c48dde0e06e2de53f80f21123a3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:48:51 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 21 Feb 2020 22:48:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:56 GMT
ENV MONGO_MAJOR=3.6
# Fri, 21 Feb 2020 22:48:57 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 21 Feb 2020 22:48:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 21 Feb 2020 22:49:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 21 Feb 2020 22:49:23 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 21 Feb 2020 22:49:24 GMT
VOLUME [/data/db /data/configdb]
# Fri, 21 Feb 2020 22:49:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 21 Feb 2020 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 22:49:26 GMT
EXPOSE 27017
# Fri, 21 Feb 2020 22:49:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c551726d412935a665a5faa37ba35c6b578c9b4b9a04e15fbb8141e18c469f4`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690416c5e0de4a88eb11a3f888d668dffc71c64ce9928810382a5f989ea0d6d8`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466edf90a60ac36b2e4ef9846aac45cf6dcbf6603561ff365607d6ec8e1d4333`  
		Last Modified: Fri, 21 Feb 2020 22:53:01 GMT  
		Size: 111.5 MB (111459661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a78ae9c5bd995e33cabe28ea21119ec5a46c4ecd1c7a5b80beedf81e226048`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfad788e158cc0e6900c305454fae286feb8c8e9807a24c9e4a962a22727dfc`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:0f92e13d622544ed93898c56cd2b7dc2a2cf69fcc9de3b796cc4c385bea87791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:3-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:ba754b60411d37b3518e23450efea880bd623745c95513e1e7244b252451b24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:1b06d94427570603d08e7f9a33071aaab0539d66707575f3b8e7b76380a24ef4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2358218977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57309fa6315e5238c672676014e169314f218d70fd132162c2373a2bd12181ad`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 20 Mar 2020 19:15:35 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Fri, 20 Mar 2020 19:15:36 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Fri, 20 Mar 2020 19:31:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 20 Mar 2020 19:31:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 20 Mar 2020 19:31:17 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:31:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db2f31aed49e9cb0030ddf748cfea906c9ed0ff7fe6c12cfa11f1fc149699`  
		Last Modified: Fri, 20 Mar 2020 19:32:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e7f866165ec77ae349dcee7df7aff19cf88fc1f4a4c1ecca9bc73250ba7e1`  
		Last Modified: Fri, 20 Mar 2020 19:32:40 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6998d6a77b92386b15a8e50b29e34e2c117a332a218f00ef2f073a506364d8`  
		Last Modified: Fri, 20 Mar 2020 19:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59eee255809bca8e6dba19375cfbd66867049b4f99d30c8c4e16392bbc398d`  
		Last Modified: Fri, 20 Mar 2020 19:33:03 GMT  
		Size: 92.9 MB (92874591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff0035ad869a80197aa61e6d2add4833afc12f34fe1dced383cf6e63e8f774`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26d20a4e53cfb90910cc91553d728994d8e4548b52183e9a91a7382bc9b644`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a32b0db4b6bc83248c3cd1a84dadac14fd709078dadc66ff9be2f93e046fa`  
		Last Modified: Fri, 20 Mar 2020 19:32:38 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:5b86c671b4e30d6934384b87e9e0e7ec2c1e1c995737c8f9cd64a59879627e1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:75be378bf7408fafca497a44412b86c794148b02bb8db70909a6cd8091142f8f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6182116969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f823ccfbbb7c9c01f0231b74304202f481d79a938c2e94c420c600878ca57fd`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 14:58:51 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 18 Mar 2020 14:58:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 18 Mar 2020 14:58:53 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 18 Mar 2020 15:15:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:15:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:15:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:15:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387aa7fdebeffbad002987822ff10c353f9b8c02983de325cbaf6a7053300161`  
		Last Modified: Wed, 18 Mar 2020 15:44:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a860625b805fd125437ac155828512506ea5be2777851fa88c8536aecfbd2e`  
		Last Modified: Wed, 18 Mar 2020 15:44:54 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb43cfdea3c28f5cf6ea83cdee7b2fc3934257e5629714e666815fd0748d13`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb31b37531cb46475899392f63e91242d861bcd79cf0244f149c7d37aed87811`  
		Last Modified: Wed, 18 Mar 2020 15:45:43 GMT  
		Size: 453.3 MB (453347930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd56eb11cd12d10ba9f6faab05010caff1674111d9b74ec601aad00003fef81`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb437210b88ba380306ac5eae2dd896b2fc38049083d0dccaca5a0f5acd8a6`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186a7478db2330da48548f9c1c6ca7eb566d00dcfb47c5172c6edfdb131cd369`  
		Last Modified: Wed, 18 Mar 2020 15:44:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:dbdd944e50ed4f45174aae05205e284b76166e3ac9801b6f15856b79fb3f595b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:557aaf306c611bf9cd04e69fc3174757e2ce25ecc073a88fe28dbc889f5dae9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165644020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fdbdf0f17b70466eda08d155b2f1c72bc3450d23b8a752a4a841a83d6eb76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:08:41 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Sat, 22 Feb 2020 01:08:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:08:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_MAJOR=3.6
# Sat, 22 Feb 2020 01:08:42 GMT
ENV MONGO_VERSION=3.6.17
# Sat, 22 Feb 2020 01:08:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 22 Feb 2020 01:09:04 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 22 Feb 2020 01:09:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 22 Feb 2020 01:09:05 GMT
VOLUME [/data/db /data/configdb]
# Sat, 22 Feb 2020 01:09:05 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Sat, 22 Feb 2020 01:09:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 01:09:06 GMT
EXPOSE 27017
# Sat, 22 Feb 2020 01:09:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03380f32ca06a89bb8bbb6437140f7feaa8cbc73656efd413066485af7bed9`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a38c136f14bc4cc8e7c8b75a1b58fbd13ee66ab4018835cce5deafd77e34629`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0e875b59ceec4323d6455ddef1a97e267ed64e723a3785961db869da21e662`  
		Last Modified: Sat, 22 Feb 2020 01:11:19 GMT  
		Size: 117.3 MB (117252414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f55b4999cd606166300c3bcc0c29bbdb69f9e442f652f9e2a1b037ff63069d`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc92ef8de8b080701461ef5a44e3df6e2b20f0e5d0502bc9c2f58fb0c18884c`  
		Last Modified: Sat, 22 Feb 2020 01:11:00 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8d00f2129c233839b0192bc63ad1b38d732559eb063a8c7fb6afd9b14000dfe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155054951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904d1cc8fa66fbab1604f0f278d0125cf824c48dde0e06e2de53f80f21123a3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:48:51 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 21 Feb 2020 22:48:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:48:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:48:56 GMT
ENV MONGO_MAJOR=3.6
# Fri, 21 Feb 2020 22:48:57 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 21 Feb 2020 22:48:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 21 Feb 2020 22:49:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 21 Feb 2020 22:49:23 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 21 Feb 2020 22:49:24 GMT
VOLUME [/data/db /data/configdb]
# Fri, 21 Feb 2020 22:49:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 21 Feb 2020 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 22:49:26 GMT
EXPOSE 27017
# Fri, 21 Feb 2020 22:49:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c551726d412935a665a5faa37ba35c6b578c9b4b9a04e15fbb8141e18c469f4`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690416c5e0de4a88eb11a3f888d668dffc71c64ce9928810382a5f989ea0d6d8`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466edf90a60ac36b2e4ef9846aac45cf6dcbf6603561ff365607d6ec8e1d4333`  
		Last Modified: Fri, 21 Feb 2020 22:53:01 GMT  
		Size: 111.5 MB (111459661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a78ae9c5bd995e33cabe28ea21119ec5a46c4ecd1c7a5b80beedf81e226048`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfad788e158cc0e6900c305454fae286feb8c8e9807a24c9e4a962a22727dfc`  
		Last Modified: Fri, 21 Feb 2020 22:52:33 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:58b25d51baa11a85b6aedf7c4e05710d12a27ddc2883e2692e7d58527d98bd73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:92814bb60dc673bb68b6aca0b24bcb8738d7b2c267b97ce62fa92adc3746a0ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163996237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a9a3e851586594f8b4a33dbefa090c7eebbb40383fa2608e0b7c7364181094`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:49:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:49:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:49:59 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:49:59 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:50:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:50:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:50:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:50:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:50:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:50:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:50:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:50:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7fb3809884c8771103b4475a778eb0a14b736d5f2008d7ef534950c9b6b77d`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7237292ff8a2ff64ff0898dc8792b23e5abe90bf32d14f0d4d9eb6ab9e956dd`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 3.0 MB (2982755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c936e28b5159ed9120f67cd810c0a572f58627c9eb3e557462f203be9d17ea02`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 5.8 MB (5765341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb56b127f30088448b452fd8280ab6c1bcf531e41dfe389303eda286ec9058d`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a0478af29b6c5190b926d4f569bbfa66795bef31800cca8386a2d2fe53196`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f535558aec6da346f312150c731fcd65ef98b1607d7081ce8cd3b633fb007631`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c80d404ff4d5feede174df7427b40c4ffd8d3c8f8181c2e4c68cb2aa5f04426`  
		Last Modified: Fri, 20 Mar 2020 20:51:07 GMT  
		Size: 128.5 MB (128513419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6836853ff9810bc6f4e7578599f671cee7c7b8df9c0b1253c196b530dab1a6dc`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a86198cd55d5df56dcc40bd5a884c7ac2d4c020aa0a79b5d2911eb0fb66eaa0`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dd96e839f09e9bc1dda394e0c523c8d7a21f5686d51a9bf948f3b743563bb2e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (154023152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7019388c69e05fedf71750b0d132c2c3e84d5f6fe1bf2244d899f55068b79955`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:43:33 GMT
ADD file:e4214b65d372c2f971e6544f69c465e8b1ba82290276558036047179a02ba9e3 in / 
# Fri, 20 Mar 2020 18:43:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:43:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:43:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:43:39 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:04:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:05:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:05:04 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:05:05 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:05:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:05:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:05:30 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:05:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:35 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:05:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:06:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:06:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:06:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:06:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:06:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:06:12 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:06:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b2f61026a351316126bfad6f6cac3971b3b3e928b126ac53026bb4263459d2ff`  
		Last Modified: Mon, 16 Mar 2020 15:39:01 GMT  
		Size: 23.7 MB (23720219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5538fb30c42c023ad64c0e31ce3cb02e3c4150f9ac944a46d3386b8212b80043`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 35.2 KB (35206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b05810781a3c493e08dc6e2c9b9553244f8f86248f7d709a50becbac344234`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0180a33352d6b41ad6ca5fac27544fb3c8c7cb69e67dc30bf9584b49cd3b3938`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0b30f72d9df0004fc57918dfe57c7eeaebeabedce1b354a20bc349d2aa76`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714de3905b15b668e150004bcf2748d77976414da2fa5a7196ea87aeca82c86`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 2.7 MB (2675722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24815c74c3cb52ce08542232c2e58c723ac73b61c60420ccace8b3399a06d448`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 5.3 MB (5283964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f454a9ed57c563d6bd14288e39a702a7c6a6a852faecdbab7d36c884d84139`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfa48c6b5c7715dbd1f1b427ab60a04743bf7477742270124283443a893a72`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fac47022ed7bb13268ce9fade7f3d308750b9d1eacc661c90e1d68fc491237d`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d115f8bfec9339ece1ff67ffcda9a8bd028099878c45d571d02eaf3bde900eb`  
		Last Modified: Fri, 20 Mar 2020 20:06:57 GMT  
		Size: 122.3 MB (122299165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b575d18b80362b8a2f68c48d9d64421a48debaa026b2185eefb4a1760b416f`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c7de1e8291482b3b994b78d3d37b87f6032ce85a09ea0d89ef0b796025aba`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:436fd5b2912453e5d4e29390cb17da7a00ace52c8996247b983413fe405f1e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159948196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c7cfd88398e9937dbfe6efd31bd28a38431d92433142c4814deed0560cc2cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:49:47 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 19:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:49:54 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 19:49:54 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 19:50:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 19:50:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 19:50:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 19:50:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 19:50:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 19:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 19:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 19:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 19:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 19:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 19:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5729f54883440102e557e89a75ffd9062fa2729af41cbf8802d7af5e380afe`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fcb8cac271b6ec551ae5cb48658f4b47c707598258a150facf67223938ecd`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 2.7 MB (2714542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d0826978fda94ba7ce291a76276cff0f126034c5721b20efaa806a0a56d48`  
		Last Modified: Fri, 20 Mar 2020 19:50:52 GMT  
		Size: 5.7 MB (5687237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26becd0f01982ab12a47b1eabf03602ee45c3744397e79b851b0a8c73fe1fb17`  
		Last Modified: Fri, 20 Mar 2020 19:50:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b563d50c7fb9cc0a21d05c4710f4fa20993b6406889fa7151505d04b368a57d`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e1933d9298653dfffe189d64b111aeec1cf5833b6b7c164c5ffab370609ddd`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e4d3bc43302c45fe0fdf3a81c39eb49cd1beb3cc298004c59f63f06d506c6b`  
		Last Modified: Fri, 20 Mar 2020 19:51:00 GMT  
		Size: 126.1 MB (126136771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86ac4edeadab16931b15c4eaec07a8d7ce0d50d4ff696fcdc1b429b10f88fa5`  
		Last Modified: Fri, 20 Mar 2020 19:51:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae9258b9d4657d74eda13532313b87d8ee080d201f8d149c651757e750cdb7`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:b48f20bc3cd488b4395ef7762a1e82596f7ccb5ebdd8e1eb80403afb3a7b440f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:ed9a25c3fab1742cee7c947d5b0d52e4aaab5e3b749c8e75a251e605cbdff284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153599247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6182b91a1dbea114fcf10251351db06aae502c3ecd1c132ded65106dd1e2fd6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:09:18 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 22 Feb 2020 01:09:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:09:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:09:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:09:20 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:09:20 GMT
ENV MONGO_MAJOR=4.0
# Mon, 23 Mar 2020 19:26:09 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:26:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 23 Mar 2020 19:26:42 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 23 Mar 2020 19:26:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 Mar 2020 19:26:43 GMT
VOLUME [/data/db /data/configdb]
# Mon, 23 Mar 2020 19:26:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 23 Mar 2020 19:26:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 19:26:43 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:26:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba1898ebd41f26efc884bea6eb4a7ee3ef6ce3b48ed6be03ab56b4d6621921b`  
		Last Modified: Sat, 22 Feb 2020 01:11:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d512dad9bd30e9ddd401d7aeb2f15a07b888fbca53aedb342fcffbf63ae4d`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918e8254cc4c1683695d10dc84297c63282e365d34f14b5fc1a4146c358ef39d`  
		Last Modified: Mon, 23 Mar 2020 19:27:15 GMT  
		Size: 105.2 MB (105208204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce964b5c6ad1e8f653de9a34092dbe3d094605bedde67208bc93d44a2c3e52c`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd3f1f5e6b9a96bd9d29b5885e000ee642453c8a6c2dfde39f1f3c6d8499ac`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ed10057ca758875b84838b13666bb93e7de94456776233438aa93c098edf046b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143228681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee79e73e4aba21b9d77b34465ef15826ebf5dcb9dfa3e313727170fe60e8e5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:49:43 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 21 Feb 2020 22:49:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:49:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:49:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:49:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:49:48 GMT
ENV MONGO_MAJOR=4.0
# Mon, 23 Mar 2020 19:55:33 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:55:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 23 Mar 2020 19:56:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 23 Mar 2020 19:56:10 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 Mar 2020 19:56:10 GMT
VOLUME [/data/db /data/configdb]
# Mon, 23 Mar 2020 19:56:11 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 23 Mar 2020 19:56:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 19:56:12 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:56:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb69e090ce7c1babcfff2b727157954d5d146b17548d8bb27049c97f915f5cea`  
		Last Modified: Fri, 21 Feb 2020 22:53:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f299a1cf738036efceae0b92d6cba1b72a60825a54655dcacbec14e447fe0f4`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6f735cb8c660a9ade688fdd2a008cb4273c941480d746ccd18d89971da76ee`  
		Last Modified: Mon, 23 Mar 2020 19:57:01 GMT  
		Size: 99.6 MB (99633956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07e70b136c797c3bc612f76d04055daeeed7dec3d9af87b73d85f72649ca314`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6d0907363115bcffad800f2d570f3e6d50fe1476d9adaac3d1e2fb368e12f7`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:a4adf981dc8872bd33f96d27c43b755757a3ffe4817c5545e211e859f15d3536
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815528269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbcd2ce61f40a839d27323411dfefae3ab6d661e41ad61e2a2cc1d087dc8d551`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:22:52 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:35:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:35:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:35:38 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:35:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b593fced2de9e8c5e3aa7afcdc2b32bfa994e4f92905e91317e5b861f7abf4`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b53c19caa48907164b59cd0cfee55f937414e1637adf602258123f9e20e12e2`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b52acdc8d3146cb402d98b8c98334ccd6c56111432f01e776bf90413b0e3f3`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bc1023411c163ae7ef75225f6708377da7b937284c2e42c62f2747cce2818a`  
		Last Modified: Mon, 23 Mar 2020 19:54:28 GMT  
		Size: 86.8 MB (86759287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ad6015e69444c139df03e70328183cbb51c9556e74af9f410530efe2cfc399`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfc2155afb984e21df162e6782568be4bd7721984ce4fa8a38342750f36a4e1`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b449232eddef0941562b5c9bde12e3e7fe42ebac700daad84447b3beb680fe`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:a2018b75db5c98dfe25b10094926af2c4e89c3645a807ecce0693d265010977e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2711020338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e535dcc99d5488a0b6cc2d8cc3bc6ceb6bbb4a248847f9b0085099500ec25`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:35:53 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:53:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:53:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:53:06 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:53:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f1a3463d821c763bc612de8773ea253caacb75c4c6324282bf9107b7537ddb`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06dfaf27cd9f470fc6dc270ecd2175de696aff40c2be662a58396c31eae7f16`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501be6a5bda413cabe4aba8dee6b4bd026772b22aa0c23ba3a6a39fc446a4229`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d9f3cc68c4be2017c608f0e4cd7ed0770c9936f87f0e8ccc9a6a4b1efc0a0`  
		Last Modified: Mon, 23 Mar 2020 19:55:33 GMT  
		Size: 445.7 MB (445676042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350decaed06f27679d2be2d856fc63d59fd07d5a347f280cc77a17a78b676961`  
		Last Modified: Mon, 23 Mar 2020 19:54:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b7924e5b9b4dc2e2253a993a4b53737f2d12756b1bc1dabfa6d94f4041d09`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d18e227af8263bddef1adb40c7623c1b7609c88d418887971b20d8afebe49c`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.17`

```console
$ docker pull mongo@sha256:b48f20bc3cd488b4395ef7762a1e82596f7ccb5ebdd8e1eb80403afb3a7b440f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.0.17` - linux; amd64

```console
$ docker pull mongo@sha256:ed9a25c3fab1742cee7c947d5b0d52e4aaab5e3b749c8e75a251e605cbdff284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153599247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6182b91a1dbea114fcf10251351db06aae502c3ecd1c132ded65106dd1e2fd6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:09:18 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 22 Feb 2020 01:09:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:09:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:09:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:09:20 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:09:20 GMT
ENV MONGO_MAJOR=4.0
# Mon, 23 Mar 2020 19:26:09 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:26:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 23 Mar 2020 19:26:42 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 23 Mar 2020 19:26:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 Mar 2020 19:26:43 GMT
VOLUME [/data/db /data/configdb]
# Mon, 23 Mar 2020 19:26:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 23 Mar 2020 19:26:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 19:26:43 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:26:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba1898ebd41f26efc884bea6eb4a7ee3ef6ce3b48ed6be03ab56b4d6621921b`  
		Last Modified: Sat, 22 Feb 2020 01:11:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d512dad9bd30e9ddd401d7aeb2f15a07b888fbca53aedb342fcffbf63ae4d`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918e8254cc4c1683695d10dc84297c63282e365d34f14b5fc1a4146c358ef39d`  
		Last Modified: Mon, 23 Mar 2020 19:27:15 GMT  
		Size: 105.2 MB (105208204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce964b5c6ad1e8f653de9a34092dbe3d094605bedde67208bc93d44a2c3e52c`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd3f1f5e6b9a96bd9d29b5885e000ee642453c8a6c2dfde39f1f3c6d8499ac`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.17` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ed10057ca758875b84838b13666bb93e7de94456776233438aa93c098edf046b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143228681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee79e73e4aba21b9d77b34465ef15826ebf5dcb9dfa3e313727170fe60e8e5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:49:43 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 21 Feb 2020 22:49:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:49:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:49:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:49:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:49:48 GMT
ENV MONGO_MAJOR=4.0
# Mon, 23 Mar 2020 19:55:33 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:55:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 23 Mar 2020 19:56:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 23 Mar 2020 19:56:10 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 Mar 2020 19:56:10 GMT
VOLUME [/data/db /data/configdb]
# Mon, 23 Mar 2020 19:56:11 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 23 Mar 2020 19:56:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 19:56:12 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:56:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb69e090ce7c1babcfff2b727157954d5d146b17548d8bb27049c97f915f5cea`  
		Last Modified: Fri, 21 Feb 2020 22:53:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f299a1cf738036efceae0b92d6cba1b72a60825a54655dcacbec14e447fe0f4`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6f735cb8c660a9ade688fdd2a008cb4273c941480d746ccd18d89971da76ee`  
		Last Modified: Mon, 23 Mar 2020 19:57:01 GMT  
		Size: 99.6 MB (99633956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07e70b136c797c3bc612f76d04055daeeed7dec3d9af87b73d85f72649ca314`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6d0907363115bcffad800f2d570f3e6d50fe1476d9adaac3d1e2fb368e12f7`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.17` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:a4adf981dc8872bd33f96d27c43b755757a3ffe4817c5545e211e859f15d3536
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815528269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbcd2ce61f40a839d27323411dfefae3ab6d661e41ad61e2a2cc1d087dc8d551`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:22:52 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:35:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:35:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:35:38 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:35:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b593fced2de9e8c5e3aa7afcdc2b32bfa994e4f92905e91317e5b861f7abf4`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b53c19caa48907164b59cd0cfee55f937414e1637adf602258123f9e20e12e2`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b52acdc8d3146cb402d98b8c98334ccd6c56111432f01e776bf90413b0e3f3`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bc1023411c163ae7ef75225f6708377da7b937284c2e42c62f2747cce2818a`  
		Last Modified: Mon, 23 Mar 2020 19:54:28 GMT  
		Size: 86.8 MB (86759287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ad6015e69444c139df03e70328183cbb51c9556e74af9f410530efe2cfc399`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfc2155afb984e21df162e6782568be4bd7721984ce4fa8a38342750f36a4e1`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b449232eddef0941562b5c9bde12e3e7fe42ebac700daad84447b3beb680fe`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.17` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:a2018b75db5c98dfe25b10094926af2c4e89c3645a807ecce0693d265010977e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2711020338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e535dcc99d5488a0b6cc2d8cc3bc6ceb6bbb4a248847f9b0085099500ec25`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:35:53 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:53:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:53:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:53:06 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:53:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f1a3463d821c763bc612de8773ea253caacb75c4c6324282bf9107b7537ddb`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06dfaf27cd9f470fc6dc270ecd2175de696aff40c2be662a58396c31eae7f16`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501be6a5bda413cabe4aba8dee6b4bd026772b22aa0c23ba3a6a39fc446a4229`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d9f3cc68c4be2017c608f0e4cd7ed0770c9936f87f0e8ccc9a6a4b1efc0a0`  
		Last Modified: Mon, 23 Mar 2020 19:55:33 GMT  
		Size: 445.7 MB (445676042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350decaed06f27679d2be2d856fc63d59fd07d5a347f280cc77a17a78b676961`  
		Last Modified: Mon, 23 Mar 2020 19:54:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b7924e5b9b4dc2e2253a993a4b53737f2d12756b1bc1dabfa6d94f4041d09`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d18e227af8263bddef1adb40c7623c1b7609c88d418887971b20d8afebe49c`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.17-windowsservercore`

```console
$ docker pull mongo@sha256:67add7c16ffb57082fb9cf07cb14a3485401e341bad12b95bb24582772b99919
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.0.17-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:a4adf981dc8872bd33f96d27c43b755757a3ffe4817c5545e211e859f15d3536
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815528269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbcd2ce61f40a839d27323411dfefae3ab6d661e41ad61e2a2cc1d087dc8d551`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:22:52 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:35:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:35:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:35:38 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:35:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b593fced2de9e8c5e3aa7afcdc2b32bfa994e4f92905e91317e5b861f7abf4`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b53c19caa48907164b59cd0cfee55f937414e1637adf602258123f9e20e12e2`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b52acdc8d3146cb402d98b8c98334ccd6c56111432f01e776bf90413b0e3f3`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bc1023411c163ae7ef75225f6708377da7b937284c2e42c62f2747cce2818a`  
		Last Modified: Mon, 23 Mar 2020 19:54:28 GMT  
		Size: 86.8 MB (86759287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ad6015e69444c139df03e70328183cbb51c9556e74af9f410530efe2cfc399`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfc2155afb984e21df162e6782568be4bd7721984ce4fa8a38342750f36a4e1`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b449232eddef0941562b5c9bde12e3e7fe42ebac700daad84447b3beb680fe`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.17-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:a2018b75db5c98dfe25b10094926af2c4e89c3645a807ecce0693d265010977e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2711020338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e535dcc99d5488a0b6cc2d8cc3bc6ceb6bbb4a248847f9b0085099500ec25`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:35:53 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:53:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:53:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:53:06 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:53:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f1a3463d821c763bc612de8773ea253caacb75c4c6324282bf9107b7537ddb`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06dfaf27cd9f470fc6dc270ecd2175de696aff40c2be662a58396c31eae7f16`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501be6a5bda413cabe4aba8dee6b4bd026772b22aa0c23ba3a6a39fc446a4229`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d9f3cc68c4be2017c608f0e4cd7ed0770c9936f87f0e8ccc9a6a4b1efc0a0`  
		Last Modified: Mon, 23 Mar 2020 19:55:33 GMT  
		Size: 445.7 MB (445676042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350decaed06f27679d2be2d856fc63d59fd07d5a347f280cc77a17a78b676961`  
		Last Modified: Mon, 23 Mar 2020 19:54:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b7924e5b9b4dc2e2253a993a4b53737f2d12756b1bc1dabfa6d94f4041d09`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d18e227af8263bddef1adb40c7623c1b7609c88d418887971b20d8afebe49c`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.17-windowsservercore-1809`

```console
$ docker pull mongo@sha256:8d2bff1064b89362a1863eb680f5dfe5687c658dbeac96b841133e5db7112ab4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.0.17-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:a2018b75db5c98dfe25b10094926af2c4e89c3645a807ecce0693d265010977e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2711020338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e535dcc99d5488a0b6cc2d8cc3bc6ceb6bbb4a248847f9b0085099500ec25`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:35:53 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:53:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:53:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:53:06 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:53:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f1a3463d821c763bc612de8773ea253caacb75c4c6324282bf9107b7537ddb`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06dfaf27cd9f470fc6dc270ecd2175de696aff40c2be662a58396c31eae7f16`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501be6a5bda413cabe4aba8dee6b4bd026772b22aa0c23ba3a6a39fc446a4229`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d9f3cc68c4be2017c608f0e4cd7ed0770c9936f87f0e8ccc9a6a4b1efc0a0`  
		Last Modified: Mon, 23 Mar 2020 19:55:33 GMT  
		Size: 445.7 MB (445676042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350decaed06f27679d2be2d856fc63d59fd07d5a347f280cc77a17a78b676961`  
		Last Modified: Mon, 23 Mar 2020 19:54:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b7924e5b9b4dc2e2253a993a4b53737f2d12756b1bc1dabfa6d94f4041d09`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d18e227af8263bddef1adb40c7623c1b7609c88d418887971b20d8afebe49c`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.17-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:88c86a30c3d5589e1de85d04906be6741a7ade17bdacd3476a56567b6b4a3850
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:4.0.17-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:a4adf981dc8872bd33f96d27c43b755757a3ffe4817c5545e211e859f15d3536
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815528269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbcd2ce61f40a839d27323411dfefae3ab6d661e41ad61e2a2cc1d087dc8d551`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:22:52 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:35:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:35:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:35:38 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:35:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b593fced2de9e8c5e3aa7afcdc2b32bfa994e4f92905e91317e5b861f7abf4`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b53c19caa48907164b59cd0cfee55f937414e1637adf602258123f9e20e12e2`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b52acdc8d3146cb402d98b8c98334ccd6c56111432f01e776bf90413b0e3f3`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bc1023411c163ae7ef75225f6708377da7b937284c2e42c62f2747cce2818a`  
		Last Modified: Mon, 23 Mar 2020 19:54:28 GMT  
		Size: 86.8 MB (86759287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ad6015e69444c139df03e70328183cbb51c9556e74af9f410530efe2cfc399`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfc2155afb984e21df162e6782568be4bd7721984ce4fa8a38342750f36a4e1`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b449232eddef0941562b5c9bde12e3e7fe42ebac700daad84447b3beb680fe`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.17-xenial`

```console
$ docker pull mongo@sha256:329633dae91fa2b3a68c2f4ae0848fded3d2cee4912477fd0effc4579f845845
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.17-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:ed9a25c3fab1742cee7c947d5b0d52e4aaab5e3b749c8e75a251e605cbdff284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153599247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6182b91a1dbea114fcf10251351db06aae502c3ecd1c132ded65106dd1e2fd6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:09:18 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 22 Feb 2020 01:09:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:09:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:09:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:09:20 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:09:20 GMT
ENV MONGO_MAJOR=4.0
# Mon, 23 Mar 2020 19:26:09 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:26:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 23 Mar 2020 19:26:42 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 23 Mar 2020 19:26:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 Mar 2020 19:26:43 GMT
VOLUME [/data/db /data/configdb]
# Mon, 23 Mar 2020 19:26:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 23 Mar 2020 19:26:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 19:26:43 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:26:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba1898ebd41f26efc884bea6eb4a7ee3ef6ce3b48ed6be03ab56b4d6621921b`  
		Last Modified: Sat, 22 Feb 2020 01:11:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d512dad9bd30e9ddd401d7aeb2f15a07b888fbca53aedb342fcffbf63ae4d`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918e8254cc4c1683695d10dc84297c63282e365d34f14b5fc1a4146c358ef39d`  
		Last Modified: Mon, 23 Mar 2020 19:27:15 GMT  
		Size: 105.2 MB (105208204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce964b5c6ad1e8f653de9a34092dbe3d094605bedde67208bc93d44a2c3e52c`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd3f1f5e6b9a96bd9d29b5885e000ee642453c8a6c2dfde39f1f3c6d8499ac`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.17-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ed10057ca758875b84838b13666bb93e7de94456776233438aa93c098edf046b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143228681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee79e73e4aba21b9d77b34465ef15826ebf5dcb9dfa3e313727170fe60e8e5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:49:43 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 21 Feb 2020 22:49:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:49:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:49:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:49:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:49:48 GMT
ENV MONGO_MAJOR=4.0
# Mon, 23 Mar 2020 19:55:33 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:55:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 23 Mar 2020 19:56:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 23 Mar 2020 19:56:10 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 Mar 2020 19:56:10 GMT
VOLUME [/data/db /data/configdb]
# Mon, 23 Mar 2020 19:56:11 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 23 Mar 2020 19:56:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 19:56:12 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:56:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb69e090ce7c1babcfff2b727157954d5d146b17548d8bb27049c97f915f5cea`  
		Last Modified: Fri, 21 Feb 2020 22:53:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f299a1cf738036efceae0b92d6cba1b72a60825a54655dcacbec14e447fe0f4`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6f735cb8c660a9ade688fdd2a008cb4273c941480d746ccd18d89971da76ee`  
		Last Modified: Mon, 23 Mar 2020 19:57:01 GMT  
		Size: 99.6 MB (99633956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07e70b136c797c3bc612f76d04055daeeed7dec3d9af87b73d85f72649ca314`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6d0907363115bcffad800f2d570f3e6d50fe1476d9adaac3d1e2fb368e12f7`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:67add7c16ffb57082fb9cf07cb14a3485401e341bad12b95bb24582772b99919
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:a4adf981dc8872bd33f96d27c43b755757a3ffe4817c5545e211e859f15d3536
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815528269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbcd2ce61f40a839d27323411dfefae3ab6d661e41ad61e2a2cc1d087dc8d551`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:22:52 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:35:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:35:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:35:38 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:35:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b593fced2de9e8c5e3aa7afcdc2b32bfa994e4f92905e91317e5b861f7abf4`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b53c19caa48907164b59cd0cfee55f937414e1637adf602258123f9e20e12e2`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b52acdc8d3146cb402d98b8c98334ccd6c56111432f01e776bf90413b0e3f3`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bc1023411c163ae7ef75225f6708377da7b937284c2e42c62f2747cce2818a`  
		Last Modified: Mon, 23 Mar 2020 19:54:28 GMT  
		Size: 86.8 MB (86759287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ad6015e69444c139df03e70328183cbb51c9556e74af9f410530efe2cfc399`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfc2155afb984e21df162e6782568be4bd7721984ce4fa8a38342750f36a4e1`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b449232eddef0941562b5c9bde12e3e7fe42ebac700daad84447b3beb680fe`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:a2018b75db5c98dfe25b10094926af2c4e89c3645a807ecce0693d265010977e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2711020338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e535dcc99d5488a0b6cc2d8cc3bc6ceb6bbb4a248847f9b0085099500ec25`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:35:53 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:53:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:53:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:53:06 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:53:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f1a3463d821c763bc612de8773ea253caacb75c4c6324282bf9107b7537ddb`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06dfaf27cd9f470fc6dc270ecd2175de696aff40c2be662a58396c31eae7f16`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501be6a5bda413cabe4aba8dee6b4bd026772b22aa0c23ba3a6a39fc446a4229`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d9f3cc68c4be2017c608f0e4cd7ed0770c9936f87f0e8ccc9a6a4b1efc0a0`  
		Last Modified: Mon, 23 Mar 2020 19:55:33 GMT  
		Size: 445.7 MB (445676042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350decaed06f27679d2be2d856fc63d59fd07d5a347f280cc77a17a78b676961`  
		Last Modified: Mon, 23 Mar 2020 19:54:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b7924e5b9b4dc2e2253a993a4b53737f2d12756b1bc1dabfa6d94f4041d09`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d18e227af8263bddef1adb40c7623c1b7609c88d418887971b20d8afebe49c`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:8d2bff1064b89362a1863eb680f5dfe5687c658dbeac96b841133e5db7112ab4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:a2018b75db5c98dfe25b10094926af2c4e89c3645a807ecce0693d265010977e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2711020338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e535dcc99d5488a0b6cc2d8cc3bc6ceb6bbb4a248847f9b0085099500ec25`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:35:53 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:35:54 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:53:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:53:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:53:06 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:53:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f1a3463d821c763bc612de8773ea253caacb75c4c6324282bf9107b7537ddb`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06dfaf27cd9f470fc6dc270ecd2175de696aff40c2be662a58396c31eae7f16`  
		Last Modified: Mon, 23 Mar 2020 19:54:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501be6a5bda413cabe4aba8dee6b4bd026772b22aa0c23ba3a6a39fc446a4229`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d9f3cc68c4be2017c608f0e4cd7ed0770c9936f87f0e8ccc9a6a4b1efc0a0`  
		Last Modified: Mon, 23 Mar 2020 19:55:33 GMT  
		Size: 445.7 MB (445676042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350decaed06f27679d2be2d856fc63d59fd07d5a347f280cc77a17a78b676961`  
		Last Modified: Mon, 23 Mar 2020 19:54:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b7924e5b9b4dc2e2253a993a4b53737f2d12756b1bc1dabfa6d94f4041d09`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d18e227af8263bddef1adb40c7623c1b7609c88d418887971b20d8afebe49c`  
		Last Modified: Mon, 23 Mar 2020 19:54:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:88c86a30c3d5589e1de85d04906be6741a7ade17bdacd3476a56567b6b4a3850
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:a4adf981dc8872bd33f96d27c43b755757a3ffe4817c5545e211e859f15d3536
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815528269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbcd2ce61f40a839d27323411dfefae3ab6d661e41ad61e2a2cc1d087dc8d551`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 23 Mar 2020 19:22:52 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.17-signed.msi
# Mon, 23 Mar 2020 19:22:53 GMT
ENV MONGO_DOWNLOAD_SHA256=386ce5434bd2b780633e2d6cb648a3f30dfbfb429c1dd636358b098f009f34cb
# Mon, 23 Mar 2020 19:35:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 23 Mar 2020 19:35:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 23 Mar 2020 19:35:38 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:35:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b593fced2de9e8c5e3aa7afcdc2b32bfa994e4f92905e91317e5b861f7abf4`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b53c19caa48907164b59cd0cfee55f937414e1637adf602258123f9e20e12e2`  
		Last Modified: Mon, 23 Mar 2020 19:54:11 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b52acdc8d3146cb402d98b8c98334ccd6c56111432f01e776bf90413b0e3f3`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bc1023411c163ae7ef75225f6708377da7b937284c2e42c62f2747cce2818a`  
		Last Modified: Mon, 23 Mar 2020 19:54:28 GMT  
		Size: 86.8 MB (86759287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ad6015e69444c139df03e70328183cbb51c9556e74af9f410530efe2cfc399`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfc2155afb984e21df162e6782568be4bd7721984ce4fa8a38342750f36a4e1`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b449232eddef0941562b5c9bde12e3e7fe42ebac700daad84447b3beb680fe`  
		Last Modified: Mon, 23 Mar 2020 19:54:09 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:329633dae91fa2b3a68c2f4ae0848fded3d2cee4912477fd0effc4579f845845
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:ed9a25c3fab1742cee7c947d5b0d52e4aaab5e3b749c8e75a251e605cbdff284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153599247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6182b91a1dbea114fcf10251351db06aae502c3ecd1c132ded65106dd1e2fd6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 01:08:16 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 22 Feb 2020 01:08:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 01:08:24 GMT
ENV GOSU_VERSION=1.11
# Sat, 22 Feb 2020 01:08:24 GMT
ENV JSYAML_VERSION=3.13.0
# Sat, 22 Feb 2020 01:08:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 22 Feb 2020 01:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 22 Feb 2020 01:09:18 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Sat, 22 Feb 2020 01:09:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 22 Feb 2020 01:09:19 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 22 Feb 2020 01:09:19 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:09:20 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 22 Feb 2020 01:09:20 GMT
ENV MONGO_MAJOR=4.0
# Mon, 23 Mar 2020 19:26:09 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:26:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 23 Mar 2020 19:26:42 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 23 Mar 2020 19:26:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 Mar 2020 19:26:43 GMT
VOLUME [/data/db /data/configdb]
# Mon, 23 Mar 2020 19:26:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 23 Mar 2020 19:26:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 19:26:43 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:26:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f659f7c5a8a29b7c2592bc12a6afb9babe94617501a765bab59df899dfa98ac`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7ff548bb868b716a6e1ffbc5281d3f298fa1f2d6bac7843ef09901a0ee5c0`  
		Last Modified: Sat, 22 Feb 2020 01:11:02 GMT  
		Size: 2.9 MB (2946077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f706fb8c773a1773b04049e2fc1aa9f63e9f8b1ecbaae99fcf970f69c417f18`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 1.2 MB (1243833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137797464445cc1df1f6510d063791f41c4be58a91cbde2d7c9e9d5985cab6d`  
		Last Modified: Sat, 22 Feb 2020 01:11:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba1898ebd41f26efc884bea6eb4a7ee3ef6ce3b48ed6be03ab56b4d6621921b`  
		Last Modified: Sat, 22 Feb 2020 01:11:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d512dad9bd30e9ddd401d7aeb2f15a07b888fbca53aedb342fcffbf63ae4d`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918e8254cc4c1683695d10dc84297c63282e365d34f14b5fc1a4146c358ef39d`  
		Last Modified: Mon, 23 Mar 2020 19:27:15 GMT  
		Size: 105.2 MB (105208204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce964b5c6ad1e8f653de9a34092dbe3d094605bedde67208bc93d44a2c3e52c`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd3f1f5e6b9a96bd9d29b5885e000ee642453c8a6c2dfde39f1f3c6d8499ac`  
		Last Modified: Mon, 23 Mar 2020 19:26:57 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ed10057ca758875b84838b13666bb93e7de94456776233438aa93c098edf046b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143228681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee79e73e4aba21b9d77b34465ef15826ebf5dcb9dfa3e313727170fe60e8e5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:48:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 21 Feb 2020 22:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:48:17 GMT
ENV GOSU_VERSION=1.11
# Fri, 21 Feb 2020 22:48:19 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 21 Feb 2020 22:48:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 21 Feb 2020 22:48:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 22:49:43 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 21 Feb 2020 22:49:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 21 Feb 2020 22:49:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 21 Feb 2020 22:49:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:49:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 21 Feb 2020 22:49:48 GMT
ENV MONGO_MAJOR=4.0
# Mon, 23 Mar 2020 19:55:33 GMT
ENV MONGO_VERSION=4.0.17
# Mon, 23 Mar 2020 19:55:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 23 Mar 2020 19:56:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 23 Mar 2020 19:56:10 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 Mar 2020 19:56:10 GMT
VOLUME [/data/db /data/configdb]
# Mon, 23 Mar 2020 19:56:11 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Mon, 23 Mar 2020 19:56:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 19:56:12 GMT
EXPOSE 27017
# Mon, 23 Mar 2020 19:56:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b98e127168243d033826ae375801cd9bde48991cd8c3f70195b2393e612fdd`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8b81c3e37e64b559f25587bfdcb850b0f99e789d079c3a5e23aedc76a5b133`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 2.5 MB (2474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133614dc076c55be0b03423a8f81053612df19fc888c3a5e65cf096386ca61a`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 1.2 MB (1170004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa274bfc4efdade7b87ff58757777040775bd689e0478b13c0325ace270c75b`  
		Last Modified: Fri, 21 Feb 2020 22:52:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb69e090ce7c1babcfff2b727157954d5d146b17548d8bb27049c97f915f5cea`  
		Last Modified: Fri, 21 Feb 2020 22:53:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f299a1cf738036efceae0b92d6cba1b72a60825a54655dcacbec14e447fe0f4`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6f735cb8c660a9ade688fdd2a008cb4273c941480d746ccd18d89971da76ee`  
		Last Modified: Mon, 23 Mar 2020 19:57:01 GMT  
		Size: 99.6 MB (99633956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07e70b136c797c3bc612f76d04055daeeed7dec3d9af87b73d85f72649ca314`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6d0907363115bcffad800f2d570f3e6d50fe1476d9adaac3d1e2fb368e12f7`  
		Last Modified: Mon, 23 Mar 2020 19:56:35 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:58b25d51baa11a85b6aedf7c4e05710d12a27ddc2883e2692e7d58527d98bd73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:92814bb60dc673bb68b6aca0b24bcb8738d7b2c267b97ce62fa92adc3746a0ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163996237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a9a3e851586594f8b4a33dbefa090c7eebbb40383fa2608e0b7c7364181094`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:49:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:49:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:49:59 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:49:59 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:50:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:50:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:50:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:50:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:50:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:50:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:50:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:50:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7fb3809884c8771103b4475a778eb0a14b736d5f2008d7ef534950c9b6b77d`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7237292ff8a2ff64ff0898dc8792b23e5abe90bf32d14f0d4d9eb6ab9e956dd`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 3.0 MB (2982755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c936e28b5159ed9120f67cd810c0a572f58627c9eb3e557462f203be9d17ea02`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 5.8 MB (5765341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb56b127f30088448b452fd8280ab6c1bcf531e41dfe389303eda286ec9058d`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a0478af29b6c5190b926d4f569bbfa66795bef31800cca8386a2d2fe53196`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f535558aec6da346f312150c731fcd65ef98b1607d7081ce8cd3b633fb007631`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c80d404ff4d5feede174df7427b40c4ffd8d3c8f8181c2e4c68cb2aa5f04426`  
		Last Modified: Fri, 20 Mar 2020 20:51:07 GMT  
		Size: 128.5 MB (128513419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6836853ff9810bc6f4e7578599f671cee7c7b8df9c0b1253c196b530dab1a6dc`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a86198cd55d5df56dcc40bd5a884c7ac2d4c020aa0a79b5d2911eb0fb66eaa0`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dd96e839f09e9bc1dda394e0c523c8d7a21f5686d51a9bf948f3b743563bb2e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (154023152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7019388c69e05fedf71750b0d132c2c3e84d5f6fe1bf2244d899f55068b79955`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:43:33 GMT
ADD file:e4214b65d372c2f971e6544f69c465e8b1ba82290276558036047179a02ba9e3 in / 
# Fri, 20 Mar 2020 18:43:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:43:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:43:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:43:39 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:04:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:05:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:05:04 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:05:05 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:05:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:05:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:05:30 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:05:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:35 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:05:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:06:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:06:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:06:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:06:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:06:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:06:12 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:06:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b2f61026a351316126bfad6f6cac3971b3b3e928b126ac53026bb4263459d2ff`  
		Last Modified: Mon, 16 Mar 2020 15:39:01 GMT  
		Size: 23.7 MB (23720219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5538fb30c42c023ad64c0e31ce3cb02e3c4150f9ac944a46d3386b8212b80043`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 35.2 KB (35206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b05810781a3c493e08dc6e2c9b9553244f8f86248f7d709a50becbac344234`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0180a33352d6b41ad6ca5fac27544fb3c8c7cb69e67dc30bf9584b49cd3b3938`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0b30f72d9df0004fc57918dfe57c7eeaebeabedce1b354a20bc349d2aa76`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714de3905b15b668e150004bcf2748d77976414da2fa5a7196ea87aeca82c86`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 2.7 MB (2675722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24815c74c3cb52ce08542232c2e58c723ac73b61c60420ccace8b3399a06d448`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 5.3 MB (5283964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f454a9ed57c563d6bd14288e39a702a7c6a6a852faecdbab7d36c884d84139`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfa48c6b5c7715dbd1f1b427ab60a04743bf7477742270124283443a893a72`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fac47022ed7bb13268ce9fade7f3d308750b9d1eacc661c90e1d68fc491237d`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d115f8bfec9339ece1ff67ffcda9a8bd028099878c45d571d02eaf3bde900eb`  
		Last Modified: Fri, 20 Mar 2020 20:06:57 GMT  
		Size: 122.3 MB (122299165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b575d18b80362b8a2f68c48d9d64421a48debaa026b2185eefb4a1760b416f`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c7de1e8291482b3b994b78d3d37b87f6032ce85a09ea0d89ef0b796025aba`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; s390x

```console
$ docker pull mongo@sha256:436fd5b2912453e5d4e29390cb17da7a00ace52c8996247b983413fe405f1e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159948196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c7cfd88398e9937dbfe6efd31bd28a38431d92433142c4814deed0560cc2cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:49:47 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 19:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:49:54 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 19:49:54 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 19:50:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 19:50:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 19:50:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 19:50:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 19:50:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 19:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 19:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 19:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 19:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 19:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 19:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5729f54883440102e557e89a75ffd9062fa2729af41cbf8802d7af5e380afe`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fcb8cac271b6ec551ae5cb48658f4b47c707598258a150facf67223938ecd`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 2.7 MB (2714542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d0826978fda94ba7ce291a76276cff0f126034c5721b20efaa806a0a56d48`  
		Last Modified: Fri, 20 Mar 2020 19:50:52 GMT  
		Size: 5.7 MB (5687237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26becd0f01982ab12a47b1eabf03602ee45c3744397e79b851b0a8c73fe1fb17`  
		Last Modified: Fri, 20 Mar 2020 19:50:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b563d50c7fb9cc0a21d05c4710f4fa20993b6406889fa7151505d04b368a57d`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e1933d9298653dfffe189d64b111aeec1cf5833b6b7c164c5ffab370609ddd`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e4d3bc43302c45fe0fdf3a81c39eb49cd1beb3cc298004c59f63f06d506c6b`  
		Last Modified: Fri, 20 Mar 2020 19:51:00 GMT  
		Size: 126.1 MB (126136771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86ac4edeadab16931b15c4eaec07a8d7ce0d50d4ff696fcdc1b429b10f88fa5`  
		Last Modified: Fri, 20 Mar 2020 19:51:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae9258b9d4657d74eda13532313b87d8ee080d201f8d149c651757e750cdb7`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.5`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2.5-bionic`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2.5-windowsservercore`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2.5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2.5-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:bf66059c15e6162355555aa2b37ccbae05c09b8218eb0c60eca32f4ed11ca3f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:92814bb60dc673bb68b6aca0b24bcb8738d7b2c267b97ce62fa92adc3746a0ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163996237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a9a3e851586594f8b4a33dbefa090c7eebbb40383fa2608e0b7c7364181094`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:49:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:49:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:49:59 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:49:59 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:50:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:50:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:50:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:50:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:50:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:50:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:50:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:50:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7fb3809884c8771103b4475a778eb0a14b736d5f2008d7ef534950c9b6b77d`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7237292ff8a2ff64ff0898dc8792b23e5abe90bf32d14f0d4d9eb6ab9e956dd`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 3.0 MB (2982755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c936e28b5159ed9120f67cd810c0a572f58627c9eb3e557462f203be9d17ea02`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 5.8 MB (5765341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb56b127f30088448b452fd8280ab6c1bcf531e41dfe389303eda286ec9058d`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a0478af29b6c5190b926d4f569bbfa66795bef31800cca8386a2d2fe53196`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f535558aec6da346f312150c731fcd65ef98b1607d7081ce8cd3b633fb007631`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c80d404ff4d5feede174df7427b40c4ffd8d3c8f8181c2e4c68cb2aa5f04426`  
		Last Modified: Fri, 20 Mar 2020 20:51:07 GMT  
		Size: 128.5 MB (128513419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6836853ff9810bc6f4e7578599f671cee7c7b8df9c0b1253c196b530dab1a6dc`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a86198cd55d5df56dcc40bd5a884c7ac2d4c020aa0a79b5d2911eb0fb66eaa0`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dd96e839f09e9bc1dda394e0c523c8d7a21f5686d51a9bf948f3b743563bb2e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (154023152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7019388c69e05fedf71750b0d132c2c3e84d5f6fe1bf2244d899f55068b79955`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:43:33 GMT
ADD file:e4214b65d372c2f971e6544f69c465e8b1ba82290276558036047179a02ba9e3 in / 
# Fri, 20 Mar 2020 18:43:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:43:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:43:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:43:39 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:04:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:05:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:05:04 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:05:05 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:05:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:05:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:05:30 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:05:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:35 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:05:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:06:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:06:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:06:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:06:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:06:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:06:12 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:06:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b2f61026a351316126bfad6f6cac3971b3b3e928b126ac53026bb4263459d2ff`  
		Last Modified: Mon, 16 Mar 2020 15:39:01 GMT  
		Size: 23.7 MB (23720219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5538fb30c42c023ad64c0e31ce3cb02e3c4150f9ac944a46d3386b8212b80043`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 35.2 KB (35206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b05810781a3c493e08dc6e2c9b9553244f8f86248f7d709a50becbac344234`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0180a33352d6b41ad6ca5fac27544fb3c8c7cb69e67dc30bf9584b49cd3b3938`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0b30f72d9df0004fc57918dfe57c7eeaebeabedce1b354a20bc349d2aa76`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714de3905b15b668e150004bcf2748d77976414da2fa5a7196ea87aeca82c86`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 2.7 MB (2675722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24815c74c3cb52ce08542232c2e58c723ac73b61c60420ccace8b3399a06d448`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 5.3 MB (5283964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f454a9ed57c563d6bd14288e39a702a7c6a6a852faecdbab7d36c884d84139`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfa48c6b5c7715dbd1f1b427ab60a04743bf7477742270124283443a893a72`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fac47022ed7bb13268ce9fade7f3d308750b9d1eacc661c90e1d68fc491237d`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d115f8bfec9339ece1ff67ffcda9a8bd028099878c45d571d02eaf3bde900eb`  
		Last Modified: Fri, 20 Mar 2020 20:06:57 GMT  
		Size: 122.3 MB (122299165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b575d18b80362b8a2f68c48d9d64421a48debaa026b2185eefb4a1760b416f`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c7de1e8291482b3b994b78d3d37b87f6032ce85a09ea0d89ef0b796025aba`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:436fd5b2912453e5d4e29390cb17da7a00ace52c8996247b983413fe405f1e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159948196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c7cfd88398e9937dbfe6efd31bd28a38431d92433142c4814deed0560cc2cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:49:47 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 19:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:49:54 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 19:49:54 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 19:50:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 19:50:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 19:50:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 19:50:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 19:50:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 19:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 19:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 19:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 19:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 19:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 19:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5729f54883440102e557e89a75ffd9062fa2729af41cbf8802d7af5e380afe`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fcb8cac271b6ec551ae5cb48658f4b47c707598258a150facf67223938ecd`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 2.7 MB (2714542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d0826978fda94ba7ce291a76276cff0f126034c5721b20efaa806a0a56d48`  
		Last Modified: Fri, 20 Mar 2020 19:50:52 GMT  
		Size: 5.7 MB (5687237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26becd0f01982ab12a47b1eabf03602ee45c3744397e79b851b0a8c73fe1fb17`  
		Last Modified: Fri, 20 Mar 2020 19:50:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b563d50c7fb9cc0a21d05c4710f4fa20993b6406889fa7151505d04b368a57d`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e1933d9298653dfffe189d64b111aeec1cf5833b6b7c164c5ffab370609ddd`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e4d3bc43302c45fe0fdf3a81c39eb49cd1beb3cc298004c59f63f06d506c6b`  
		Last Modified: Fri, 20 Mar 2020 19:51:00 GMT  
		Size: 126.1 MB (126136771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86ac4edeadab16931b15c4eaec07a8d7ce0d50d4ff696fcdc1b429b10f88fa5`  
		Last Modified: Fri, 20 Mar 2020 19:51:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae9258b9d4657d74eda13532313b87d8ee080d201f8d149c651757e750cdb7`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:cbf77948007fc2cbbbd824c226739abe78b0c2079e47bfb59593c988d96c2704
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:d934c0075f6a09fef6cba2d002d7f37e28f70e2007cacaa1bff067a56a097e46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:6f3911add9aa740851e75774706387a3deea318474ebfd35961a72ee2dfe4baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:bf66059c15e6162355555aa2b37ccbae05c09b8218eb0c60eca32f4ed11ca3f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:92814bb60dc673bb68b6aca0b24bcb8738d7b2c267b97ce62fa92adc3746a0ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163996237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a9a3e851586594f8b4a33dbefa090c7eebbb40383fa2608e0b7c7364181094`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:49:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:49:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:49:59 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:49:59 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:50:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:50:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:50:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:50:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:50:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:50:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:50:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:50:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7fb3809884c8771103b4475a778eb0a14b736d5f2008d7ef534950c9b6b77d`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7237292ff8a2ff64ff0898dc8792b23e5abe90bf32d14f0d4d9eb6ab9e956dd`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 3.0 MB (2982755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c936e28b5159ed9120f67cd810c0a572f58627c9eb3e557462f203be9d17ea02`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 5.8 MB (5765341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb56b127f30088448b452fd8280ab6c1bcf531e41dfe389303eda286ec9058d`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a0478af29b6c5190b926d4f569bbfa66795bef31800cca8386a2d2fe53196`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f535558aec6da346f312150c731fcd65ef98b1607d7081ce8cd3b633fb007631`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c80d404ff4d5feede174df7427b40c4ffd8d3c8f8181c2e4c68cb2aa5f04426`  
		Last Modified: Fri, 20 Mar 2020 20:51:07 GMT  
		Size: 128.5 MB (128513419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6836853ff9810bc6f4e7578599f671cee7c7b8df9c0b1253c196b530dab1a6dc`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a86198cd55d5df56dcc40bd5a884c7ac2d4c020aa0a79b5d2911eb0fb66eaa0`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dd96e839f09e9bc1dda394e0c523c8d7a21f5686d51a9bf948f3b743563bb2e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (154023152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7019388c69e05fedf71750b0d132c2c3e84d5f6fe1bf2244d899f55068b79955`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:43:33 GMT
ADD file:e4214b65d372c2f971e6544f69c465e8b1ba82290276558036047179a02ba9e3 in / 
# Fri, 20 Mar 2020 18:43:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:43:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:43:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:43:39 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:04:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:05:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:05:04 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:05:05 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:05:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:05:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:05:30 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:05:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:35 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:05:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:06:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:06:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:06:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:06:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:06:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:06:12 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:06:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b2f61026a351316126bfad6f6cac3971b3b3e928b126ac53026bb4263459d2ff`  
		Last Modified: Mon, 16 Mar 2020 15:39:01 GMT  
		Size: 23.7 MB (23720219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5538fb30c42c023ad64c0e31ce3cb02e3c4150f9ac944a46d3386b8212b80043`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 35.2 KB (35206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b05810781a3c493e08dc6e2c9b9553244f8f86248f7d709a50becbac344234`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0180a33352d6b41ad6ca5fac27544fb3c8c7cb69e67dc30bf9584b49cd3b3938`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0b30f72d9df0004fc57918dfe57c7eeaebeabedce1b354a20bc349d2aa76`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714de3905b15b668e150004bcf2748d77976414da2fa5a7196ea87aeca82c86`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 2.7 MB (2675722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24815c74c3cb52ce08542232c2e58c723ac73b61c60420ccace8b3399a06d448`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 5.3 MB (5283964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f454a9ed57c563d6bd14288e39a702a7c6a6a852faecdbab7d36c884d84139`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfa48c6b5c7715dbd1f1b427ab60a04743bf7477742270124283443a893a72`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fac47022ed7bb13268ce9fade7f3d308750b9d1eacc661c90e1d68fc491237d`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d115f8bfec9339ece1ff67ffcda9a8bd028099878c45d571d02eaf3bde900eb`  
		Last Modified: Fri, 20 Mar 2020 20:06:57 GMT  
		Size: 122.3 MB (122299165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b575d18b80362b8a2f68c48d9d64421a48debaa026b2185eefb4a1760b416f`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c7de1e8291482b3b994b78d3d37b87f6032ce85a09ea0d89ef0b796025aba`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:436fd5b2912453e5d4e29390cb17da7a00ace52c8996247b983413fe405f1e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159948196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c7cfd88398e9937dbfe6efd31bd28a38431d92433142c4814deed0560cc2cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:49:47 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 19:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:49:54 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 19:49:54 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 19:50:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 19:50:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 19:50:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 19:50:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 19:50:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 19:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 19:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 19:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 19:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 19:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 19:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5729f54883440102e557e89a75ffd9062fa2729af41cbf8802d7af5e380afe`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fcb8cac271b6ec551ae5cb48658f4b47c707598258a150facf67223938ecd`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 2.7 MB (2714542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d0826978fda94ba7ce291a76276cff0f126034c5721b20efaa806a0a56d48`  
		Last Modified: Fri, 20 Mar 2020 19:50:52 GMT  
		Size: 5.7 MB (5687237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26becd0f01982ab12a47b1eabf03602ee45c3744397e79b851b0a8c73fe1fb17`  
		Last Modified: Fri, 20 Mar 2020 19:50:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b563d50c7fb9cc0a21d05c4710f4fa20993b6406889fa7151505d04b368a57d`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e1933d9298653dfffe189d64b111aeec1cf5833b6b7c164c5ffab370609ddd`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e4d3bc43302c45fe0fdf3a81c39eb49cd1beb3cc298004c59f63f06d506c6b`  
		Last Modified: Fri, 20 Mar 2020 19:51:00 GMT  
		Size: 126.1 MB (126136771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86ac4edeadab16931b15c4eaec07a8d7ce0d50d4ff696fcdc1b429b10f88fa5`  
		Last Modified: Fri, 20 Mar 2020 19:51:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae9258b9d4657d74eda13532313b87d8ee080d201f8d149c651757e750cdb7`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:cbf77948007fc2cbbbd824c226739abe78b0c2079e47bfb59593c988d96c2704
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:4-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:d934c0075f6a09fef6cba2d002d7f37e28f70e2007cacaa1bff067a56a097e46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:6f3911add9aa740851e75774706387a3deea318474ebfd35961a72ee2dfe4baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:bf66059c15e6162355555aa2b37ccbae05c09b8218eb0c60eca32f4ed11ca3f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:92814bb60dc673bb68b6aca0b24bcb8738d7b2c267b97ce62fa92adc3746a0ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163996237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a9a3e851586594f8b4a33dbefa090c7eebbb40383fa2608e0b7c7364181094`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:49:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:49:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:49:59 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:49:59 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:50:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:50:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:50:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:50:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:50:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:50:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:50:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:50:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7fb3809884c8771103b4475a778eb0a14b736d5f2008d7ef534950c9b6b77d`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7237292ff8a2ff64ff0898dc8792b23e5abe90bf32d14f0d4d9eb6ab9e956dd`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 3.0 MB (2982755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c936e28b5159ed9120f67cd810c0a572f58627c9eb3e557462f203be9d17ea02`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 5.8 MB (5765341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb56b127f30088448b452fd8280ab6c1bcf531e41dfe389303eda286ec9058d`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a0478af29b6c5190b926d4f569bbfa66795bef31800cca8386a2d2fe53196`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f535558aec6da346f312150c731fcd65ef98b1607d7081ce8cd3b633fb007631`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c80d404ff4d5feede174df7427b40c4ffd8d3c8f8181c2e4c68cb2aa5f04426`  
		Last Modified: Fri, 20 Mar 2020 20:51:07 GMT  
		Size: 128.5 MB (128513419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6836853ff9810bc6f4e7578599f671cee7c7b8df9c0b1253c196b530dab1a6dc`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a86198cd55d5df56dcc40bd5a884c7ac2d4c020aa0a79b5d2911eb0fb66eaa0`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dd96e839f09e9bc1dda394e0c523c8d7a21f5686d51a9bf948f3b743563bb2e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (154023152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7019388c69e05fedf71750b0d132c2c3e84d5f6fe1bf2244d899f55068b79955`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:43:33 GMT
ADD file:e4214b65d372c2f971e6544f69c465e8b1ba82290276558036047179a02ba9e3 in / 
# Fri, 20 Mar 2020 18:43:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:43:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:43:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:43:39 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:04:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:05:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:05:04 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:05:05 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:05:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:05:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:05:30 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:05:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:35 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:05:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:06:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:06:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:06:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:06:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:06:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:06:12 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:06:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b2f61026a351316126bfad6f6cac3971b3b3e928b126ac53026bb4263459d2ff`  
		Last Modified: Mon, 16 Mar 2020 15:39:01 GMT  
		Size: 23.7 MB (23720219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5538fb30c42c023ad64c0e31ce3cb02e3c4150f9ac944a46d3386b8212b80043`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 35.2 KB (35206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b05810781a3c493e08dc6e2c9b9553244f8f86248f7d709a50becbac344234`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0180a33352d6b41ad6ca5fac27544fb3c8c7cb69e67dc30bf9584b49cd3b3938`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0b30f72d9df0004fc57918dfe57c7eeaebeabedce1b354a20bc349d2aa76`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714de3905b15b668e150004bcf2748d77976414da2fa5a7196ea87aeca82c86`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 2.7 MB (2675722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24815c74c3cb52ce08542232c2e58c723ac73b61c60420ccace8b3399a06d448`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 5.3 MB (5283964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f454a9ed57c563d6bd14288e39a702a7c6a6a852faecdbab7d36c884d84139`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfa48c6b5c7715dbd1f1b427ab60a04743bf7477742270124283443a893a72`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fac47022ed7bb13268ce9fade7f3d308750b9d1eacc661c90e1d68fc491237d`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d115f8bfec9339ece1ff67ffcda9a8bd028099878c45d571d02eaf3bde900eb`  
		Last Modified: Fri, 20 Mar 2020 20:06:57 GMT  
		Size: 122.3 MB (122299165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b575d18b80362b8a2f68c48d9d64421a48debaa026b2185eefb4a1760b416f`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c7de1e8291482b3b994b78d3d37b87f6032ce85a09ea0d89ef0b796025aba`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:436fd5b2912453e5d4e29390cb17da7a00ace52c8996247b983413fe405f1e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159948196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c7cfd88398e9937dbfe6efd31bd28a38431d92433142c4814deed0560cc2cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:49:47 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 19:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:49:54 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 19:49:54 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 19:50:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 19:50:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 19:50:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 19:50:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 19:50:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 19:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 19:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 19:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 19:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 19:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 19:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5729f54883440102e557e89a75ffd9062fa2729af41cbf8802d7af5e380afe`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fcb8cac271b6ec551ae5cb48658f4b47c707598258a150facf67223938ecd`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 2.7 MB (2714542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d0826978fda94ba7ce291a76276cff0f126034c5721b20efaa806a0a56d48`  
		Last Modified: Fri, 20 Mar 2020 19:50:52 GMT  
		Size: 5.7 MB (5687237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26becd0f01982ab12a47b1eabf03602ee45c3744397e79b851b0a8c73fe1fb17`  
		Last Modified: Fri, 20 Mar 2020 19:50:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b563d50c7fb9cc0a21d05c4710f4fa20993b6406889fa7151505d04b368a57d`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e1933d9298653dfffe189d64b111aeec1cf5833b6b7c164c5ffab370609ddd`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e4d3bc43302c45fe0fdf3a81c39eb49cd1beb3cc298004c59f63f06d506c6b`  
		Last Modified: Fri, 20 Mar 2020 19:51:00 GMT  
		Size: 126.1 MB (126136771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86ac4edeadab16931b15c4eaec07a8d7ce0d50d4ff696fcdc1b429b10f88fa5`  
		Last Modified: Fri, 20 Mar 2020 19:51:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae9258b9d4657d74eda13532313b87d8ee080d201f8d149c651757e750cdb7`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:58b25d51baa11a85b6aedf7c4e05710d12a27ddc2883e2692e7d58527d98bd73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:92814bb60dc673bb68b6aca0b24bcb8738d7b2c267b97ce62fa92adc3746a0ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163996237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a9a3e851586594f8b4a33dbefa090c7eebbb40383fa2608e0b7c7364181094`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:49:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:49:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:49:59 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:49:59 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:50:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:50:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:50:10 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:50:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:50:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:50:12 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:50:12 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:50:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:50:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7fb3809884c8771103b4475a778eb0a14b736d5f2008d7ef534950c9b6b77d`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7237292ff8a2ff64ff0898dc8792b23e5abe90bf32d14f0d4d9eb6ab9e956dd`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 3.0 MB (2982755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c936e28b5159ed9120f67cd810c0a572f58627c9eb3e557462f203be9d17ea02`  
		Last Modified: Fri, 20 Mar 2020 20:50:51 GMT  
		Size: 5.8 MB (5765341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb56b127f30088448b452fd8280ab6c1bcf531e41dfe389303eda286ec9058d`  
		Last Modified: Fri, 20 Mar 2020 20:50:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a0478af29b6c5190b926d4f569bbfa66795bef31800cca8386a2d2fe53196`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f535558aec6da346f312150c731fcd65ef98b1607d7081ce8cd3b633fb007631`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c80d404ff4d5feede174df7427b40c4ffd8d3c8f8181c2e4c68cb2aa5f04426`  
		Last Modified: Fri, 20 Mar 2020 20:51:07 GMT  
		Size: 128.5 MB (128513419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6836853ff9810bc6f4e7578599f671cee7c7b8df9c0b1253c196b530dab1a6dc`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a86198cd55d5df56dcc40bd5a884c7ac2d4c020aa0a79b5d2911eb0fb66eaa0`  
		Last Modified: Fri, 20 Mar 2020 20:50:49 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dd96e839f09e9bc1dda394e0c523c8d7a21f5686d51a9bf948f3b743563bb2e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (154023152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7019388c69e05fedf71750b0d132c2c3e84d5f6fe1bf2244d899f55068b79955`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:43:33 GMT
ADD file:e4214b65d372c2f971e6544f69c465e8b1ba82290276558036047179a02ba9e3 in / 
# Fri, 20 Mar 2020 18:43:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:43:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:43:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:43:39 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:04:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 20:05:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:05:04 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 20:05:05 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 20:05:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 20:05:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 20:05:30 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 20:05:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 20:05:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:35 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 20:05:36 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 20:05:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 20:06:07 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 20:06:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 20:06:10 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 20:06:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 20:06:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 20:06:12 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 20:06:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b2f61026a351316126bfad6f6cac3971b3b3e928b126ac53026bb4263459d2ff`  
		Last Modified: Mon, 16 Mar 2020 15:39:01 GMT  
		Size: 23.7 MB (23720219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5538fb30c42c023ad64c0e31ce3cb02e3c4150f9ac944a46d3386b8212b80043`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 35.2 KB (35206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b05810781a3c493e08dc6e2c9b9553244f8f86248f7d709a50becbac344234`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0180a33352d6b41ad6ca5fac27544fb3c8c7cb69e67dc30bf9584b49cd3b3938`  
		Last Modified: Fri, 20 Mar 2020 18:45:00 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0b30f72d9df0004fc57918dfe57c7eeaebeabedce1b354a20bc349d2aa76`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714de3905b15b668e150004bcf2748d77976414da2fa5a7196ea87aeca82c86`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 2.7 MB (2675722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24815c74c3cb52ce08542232c2e58c723ac73b61c60420ccace8b3399a06d448`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 5.3 MB (5283964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f454a9ed57c563d6bd14288e39a702a7c6a6a852faecdbab7d36c884d84139`  
		Last Modified: Fri, 20 Mar 2020 20:06:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfa48c6b5c7715dbd1f1b427ab60a04743bf7477742270124283443a893a72`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fac47022ed7bb13268ce9fade7f3d308750b9d1eacc661c90e1d68fc491237d`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d115f8bfec9339ece1ff67ffcda9a8bd028099878c45d571d02eaf3bde900eb`  
		Last Modified: Fri, 20 Mar 2020 20:06:57 GMT  
		Size: 122.3 MB (122299165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b575d18b80362b8a2f68c48d9d64421a48debaa026b2185eefb4a1760b416f`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c7de1e8291482b3b994b78d3d37b87f6032ce85a09ea0d89ef0b796025aba`  
		Last Modified: Fri, 20 Mar 2020 20:06:29 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:436fd5b2912453e5d4e29390cb17da7a00ace52c8996247b983413fe405f1e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159948196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c7cfd88398e9937dbfe6efd31bd28a38431d92433142c4814deed0560cc2cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:49:47 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 20 Mar 2020 19:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:49:54 GMT
ENV GOSU_VERSION=1.11
# Fri, 20 Mar 2020 19:49:54 GMT
ENV JSYAML_VERSION=3.13.0
# Fri, 20 Mar 2020 19:50:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 19:50:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 20 Mar 2020 19:50:06 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 20 Mar 2020 19:50:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 20 Mar 2020 19:50:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_MAJOR=4.2
# Fri, 20 Mar 2020 19:50:08 GMT
ENV MONGO_VERSION=4.2.3
# Fri, 20 Mar 2020 19:50:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 20 Mar 2020 19:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 20 Mar 2020 19:50:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 20 Mar 2020 19:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 20 Mar 2020 19:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 20 Mar 2020 19:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 19:50:32 GMT
EXPOSE 27017
# Fri, 20 Mar 2020 19:50:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5729f54883440102e557e89a75ffd9062fa2729af41cbf8802d7af5e380afe`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fcb8cac271b6ec551ae5cb48658f4b47c707598258a150facf67223938ecd`  
		Last Modified: Fri, 20 Mar 2020 19:50:48 GMT  
		Size: 2.7 MB (2714542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d0826978fda94ba7ce291a76276cff0f126034c5721b20efaa806a0a56d48`  
		Last Modified: Fri, 20 Mar 2020 19:50:52 GMT  
		Size: 5.7 MB (5687237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26becd0f01982ab12a47b1eabf03602ee45c3744397e79b851b0a8c73fe1fb17`  
		Last Modified: Fri, 20 Mar 2020 19:50:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b563d50c7fb9cc0a21d05c4710f4fa20993b6406889fa7151505d04b368a57d`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e1933d9298653dfffe189d64b111aeec1cf5833b6b7c164c5ffab370609ddd`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e4d3bc43302c45fe0fdf3a81c39eb49cd1beb3cc298004c59f63f06d506c6b`  
		Last Modified: Fri, 20 Mar 2020 19:51:00 GMT  
		Size: 126.1 MB (126136771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86ac4edeadab16931b15c4eaec07a8d7ce0d50d4ff696fcdc1b429b10f88fa5`  
		Last Modified: Fri, 20 Mar 2020 19:51:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae9258b9d4657d74eda13532313b87d8ee080d201f8d149c651757e750cdb7`  
		Last Modified: Fri, 20 Mar 2020 19:50:46 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:cbf77948007fc2cbbbd824c226739abe78b0c2079e47bfb59593c988d96c2704
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:d934c0075f6a09fef6cba2d002d7f37e28f70e2007cacaa1bff067a56a097e46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:aac754de81af2f5d162c77a945382332cffd5575897c7601ef472343cb844896
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720597037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d0aaebe9da6481c2ac37ceef6336551122a88bb8c6e0f0273b2b1408c89f3a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 23:17:35 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 11 Mar 2020 23:17:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 11 Mar 2020 23:17:37 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 11 Mar 2020 23:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 23:37:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Mar 2020 23:37:08 GMT
EXPOSE 27017
# Wed, 11 Mar 2020 23:37:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a556cdd1dac3043338300637cf3645822f875ee02355952ab1cd7751e1b68bc`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc51a0e27cfe040ead7b64a7c6a800c4c738b534689744bc5736c486935beb`  
		Last Modified: Wed, 11 Mar 2020 23:41:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f7203b7c8fc0a4e01010792bc0a916bb1d80725bd8a4e8f11428ee3160d35f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af9a292df27880e2bdab8b6325e55b0ca496959f7b3cbc864addc1d08d102d`  
		Last Modified: Wed, 11 Mar 2020 23:42:15 GMT  
		Size: 455.3 MB (455252292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb17de172b016b72e14b1ad1dc7b0d91f65115cd25a7268d5758b93956a3298f`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4339164f7d75bf46ec45b216b30960178423acd470a8d3f7fa23bcadb1e05`  
		Last Modified: Wed, 11 Mar 2020 23:41:07 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29d93e6248494f3397e2328ebfe14d053d0679135d2853daa7460ecf197df7`  
		Last Modified: Wed, 11 Mar 2020 23:41:08 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:6f3911add9aa740851e75774706387a3deea318474ebfd35961a72ee2dfe4baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:51247f0989f85aa06282e26bdef38ef82bd090adf0080f1890eac6f8bdf77d40
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825104776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edaab6ef371408b1619dc10527640da55e7c27b4fe99f1046bcbbe832d212b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 15:29:30 GMT
ENV MONGO_VERSION=4.2.3
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3-signed.msi
# Wed, 18 Mar 2020 15:29:31 GMT
ENV MONGO_DOWNLOAD_SHA256=234f6abf9c4947df94428f6ce648905dbf6b1269f48cc3239ebd4990bde1ca2a
# Wed, 18 Mar 2020 15:44:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 15:44:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Mar 2020 15:44:04 GMT
EXPOSE 27017
# Wed, 18 Mar 2020 15:44:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999df35d8fb5dd399c53e54439a7db91402a4bf545c8c889d72d501b9a9c562`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ff07621b1d4312c93fcd13fc9ebdca8bd52201578b10f463790495782d6a1`  
		Last Modified: Wed, 18 Mar 2020 15:47:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc198f35743e5d704adf34dd765aebd5e4426126c09a9f129b22bbdc2c768c`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b279b4fc5a5007413ec72b594d1edcaeef1cc46d3a433a43680f719168100`  
		Last Modified: Wed, 18 Mar 2020 15:47:57 GMT  
		Size: 96.3 MB (96335695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e01bd5719c67eaa1dd3048c9e79e2a33d92115d882caa5a8912a1a266abe3`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de485c8b832707950af0e576071151f000a5956c57fc0a4e724b41c3e027fc8`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ce79855eb1f746b2d2c30400b9e49d94f7682f5cbf08584851cb33cc859bab`  
		Last Modified: Wed, 18 Mar 2020 15:47:37 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
